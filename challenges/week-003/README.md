# Week 003: URL Shortener (In-Memory)

## Difficulty: Intermediate

## Problem

Build a URL shortener that:
1. Takes a long URL and returns a short code
2. Redirects from short code back to the original URL
3. Tracks how many times each short URL has been accessed
4. Stores everything in memory (no database needed)

## Interface

Your program should support these operations:

```
SHORTEN https://github.com/Jaidevstudio/MotherTongue
  -> abc123

RESOLVE abc123
  -> https://github.com/Jaidevstudio/MotherTongue

STATS abc123
  -> URL: https://github.com/Jaidevstudio/MotherTongue
     Short: abc123
     Visits: 3
     Created: 2026-05-08T00:00:00
```

## Implementation Options

Choose one:
- **CLI tool** -- interactive command-line interface
- **HTTP server** -- REST API with endpoints
- **Web app** -- browser-based with a form

## Bonus (Optional)

- Custom short codes: `SHORTEN https://example.com custom-name`
- Expiration: URLs expire after N hours
- QR code generation for each short URL
- Rate limiting: max 10 URLs per minute

## Constraints

- Short codes should be 6-8 characters
- Handle duplicate URLs (return existing short code)
- Validate URL format before shortening

## Submission

Create your solution in: `challenges/week-003/solutions/your-username/`
