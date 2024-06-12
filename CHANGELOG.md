# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.0] - 2024-06-07

### Added
- Initial release of the NHN Cloud Email library
  - Added `NHNCloudEmail` class with methods:
    - `send_email(recipient_email, subject, body, attachments=None)`
    - `send_bulk_email(recipient_emails, subject, body, attachments=None)`
    - `schedule_email(recipient_email, subject, body, schedule_time, attachments=None)`
    - `get_email_status(request_id)`
    - `get_sent_email_list(start_date, end_date)`
- Added `.env` file support for Email library
  - Environment variables: `NHN_CLOUD_EMAIL_APP_KEY`, `NHN_CLOUD_EMAIL_SECRET_KEY`, `NHN_CLOUD_EMAIL_SENDER`
- Comprehensive test coverage with `unittest` and support for mocking API calls using `unittest.mock`

### Changed
- None

### Fixed
- None
