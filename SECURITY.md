# Security Configuration

## Admin Credentials Setup

For security, admin credentials are now configured via environment variables instead of being hard-coded.

### Required Environment Variables

```bash
ADMIN_USERNAME=your_admin_username
ADMIN_PASSWORD=your_secure_password
SESSION_SECRET=your_random_session_secret
```

### Setup Instructions

1. Copy the example environment file:
   ```bash
   cp .env.example .env
   ```

2. Edit `.env` and set secure values:
   - `ADMIN_USERNAME`: Choose a secure admin username
   - `ADMIN_PASSWORD`: Use a strong password (minimum 12 characters)
   - `SESSION_SECRET`: Generate a random secret key

3. Restart the application to apply changes

### Password Security Best Practices

- Use passwords with at least 12 characters
- Include uppercase, lowercase, numbers, and symbols
- Avoid common words or patterns
- Consider using a password manager

### Important Notes

- Never commit `.env` files to version control
- The `.env.example` file shows the required structure but contains placeholder values
- Change the default values immediately in production environments