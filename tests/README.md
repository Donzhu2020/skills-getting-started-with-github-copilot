# FastAPI Tests

This directory contains pytest tests for the Mergington High School Activities API.

## Test Coverage

### TestGetActivities
- `test_get_activities_success` - Verifies all activities are returned
- `test_get_activities_structure` - Validates activity data structure

### TestSignupForActivity
- `test_signup_success` - Tests successful student signup
- `test_signup_duplicate` - Ensures duplicate signups are rejected
- `test_signup_nonexistent_activity` - Handles invalid activity names
- `test_signup_multiple_students` - Multiple students can join same activity

### TestUnregisterFromActivity
- `test_unregister_success` - Tests successful unregistration
- `test_unregister_not_signed_up` - Handles unregistering non-participants
- `test_unregister_nonexistent_activity` - Handles invalid activity names
- `test_signup_and_unregister_flow` - Complete signup/unregister workflow

### TestRootEndpoint
- `test_root_redirects` - Verifies root path redirects to static/index.html

## Running Tests

```bash
pytest tests/ -v
```

## Test Results

✅ All 11 tests passing
