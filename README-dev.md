# NHNCloudEmail Developer Guide

This guide is for developers contributing to the `NHNCloudEmail` library.

## Installation

To set up the development environment, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/nhncloud_email.git
    ```

2. Navigate to the project directory:
    ```bash
    cd nhncloud_email
    ```

3. Create a virtual environment:
    ```bash
    python -m venv venv
    ```

4. Activate the virtual environment:

    On Windows:
    ```bash
    venv\Scripts\activate
    ```

    On macOS/Linux:
    ```bash
    source venv/bin/activate
    ```

5. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Running Tests

Ensure all tests pass before making any changes. To run tests, use:

```bash
pytest
```


## Environment Variables
Create a .env file in the root directory with the following content:

```plaintext
NHN_CLOUD_EMAIL_APP_KEY=your_app_key
NHN_CLOUD_EMAIL_SECRET_KEY=your_secret_key
NHN_CLOUD_EMAIL_SENDER=your_sender_phone_number
```

## Building the Package
To build the package, update the version in setup.cfg:
```ini
[metadata]
name = nhncloud_email
version = x.x.x
```

Then, build the package:
```bash
python setup.py sdist bdist_wheel
```

## Deploying the Package
To deploy the package to PyPI, use Twine:
```bash
twine upload --verbose dist/nhncloud_email-x.x.x.tar.gz
```
Ensure you have the necessary permissions to upload to the PyPI repository.

## Contribution Guidelines
1. Fork the repository.
2. Create a new branch (feature/your-feature-name). 
3. Commit your changes with descriptive commit messages. 
4. Push to the branch. 
5. Create a pull request.

## Code Style
Follow PEP 8 for Python code style. Use tools like flake8 for linting and black for code formatting.

## Contact
For any questions or support, please contact dev@runners.im.

