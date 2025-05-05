# Project Design Document: Ruby on Rails Dashboard Project 1

## 1. Overview
A web application that provides users with a customizable dashboard containing:
- Weather updates
- Stock prices
- Local news
- Personal notepads

## 2. Tech Stack
- **Frontend**: Ruby on Rails (server-rendered)
- **Backend**: Rails API (if split), PostgreSQL
- **Deployment**: Render.com
- **External APIs**:
  - OpenWeatherMap (weather)
  - Yahoo Finance / Alpha Vantage (stocks)
  - News API (news)

## 3. Features
- User authentication (Devise or similar)
- User dashboard with:
  - Weather widget
  - Stock tracker
  - Local news feed
  - Notes system
- Responsive design for mobile and desktop

## 4. Database Schema (Rough Draft)
- **Users**: id, email, password_digest, created_at
- **Notes**: id, user_id, content, created_at
- (Optional) Stock and weather preferences

## 5. Routes (Initial Plan)
- `/` → Welcome page / Login
- `/dashboard` → Main dashboard (auth required)
- `/notes` → CRUD notes

## 6. Timeline / Milestones
- Week 1: Project setup, user auth
- Week 2: API integration (weather, stocks)
- Week 3: Notes system and UI polishing
- Week 4: Deployment and testing

## 7. Stretch Goals
- Drag-and-drop dashboard layout
- Dark mode toggle
- Data caching for performance

## 8. Known Challenges / Risks
- API rate limits
- OAuth for news sources (if needed)
- UI complexity if too many widgets

---

