# J-tube

A YouTube-like video sharing platform built with Spring Boot, featuring user profiles, video management, subscriptions, and social interactions.

## Tech Stack

- **Framework**: Spring Boot (REST API)
- **Security**: Spring Security 6 with role-based access control (Admin, Super Admin, User)
- **Database**: SQL database with UUID primary keys
- **Documentation**: OpenAPI/Swagger integration

## Core Features

- **User Profiles**: Registration, authentication, and profile management
- **Channels**: Create, manage, and customize creator channels with banners and descriptions
- **Video Management**: Upload, organize, and catalog videos with metadata
- **Social Interactions**: Like, dislike, and comment on videos with nested reply support
- **Subscriptions**: Subscribe/unsubscribe to channels with status tracking
- **Tags**: Organize content with tagging system
- **Watch History**: Track videos watched by users
- **Role-Based Access Control**: Admin, Super Admin, and User roles with granular permissions

## Key Endpoints

- `/video-likes` - Video engagement tracking
- `/channels` - Channel management
- `/profiles` - User profile operations
- `/subscriptions` - Channel subscriptions
- `/videos` - Video content management
- `/comments` - Video comments and replies
- `/tags` - Content categorization

## Architecture

Built with a layered architecture:
- **Controllers**: REST API endpoints with Swagger documentation
- **Services**: Business logic and CRUD operations
- **Models**: Entity classes with JPA persistence
- **Repositories**: Data access layer

## Security Features

- Spring Security integration with role-based authorization
- User authentication and session management
- Request-level access control using @PreAuthorize annotations
- Hidden fields for UUID and status tracking

## Getting Started

1. Clone the repository
2. Configure database connection
3. Run `mvn spring-boot:run`
4. Access API documentation at `/swagger-ui.html`

---

*Built as a Spring Boot learning project demonstrating REST API design, database modeling, and secure authentication patterns.*
