# Project Roadmap

This document outlines the planned milestones and future improvements for the **PlatypusBNB Backend** project.

## Milestone 1: Quality & Testing (Short-Term)
- [ ] **Automated Testing Setup**: Configure Jest and Supertest for API endpoint testing.
- [ ] **Integration Tests**: Implement integration tests for the primary endpoints:
  - `/api/stay`
  - `/api/order`
  - `/api/user`
- [ ] **CI Pipeline**: Setup GitHub Actions workflow to run ESLint and automated tests on every pull request.

## Milestone 2: API Enhancements (Medium-Term)
- [ ] **API Documentation**: Document all API endpoints using Swagger / OpenAPI.
- [ ] **Improved Validation**: Integrate `joi` or `zod` schema validation for incoming request payloads.
- [ ] **Rate Limiting**: Add rate-limiting middleware to protect public API endpoints.

## Milestone 3: Production Readiness (Long-Term)
- [ ] **Logging Service**: Enhance logging with Winston/Morgan, supporting log rotation and structured JSON output.
- [ ] **Database Optimizations**: Add indexes on frequently queried fields (e.g., stay location, user roles) to improve database query performance.
