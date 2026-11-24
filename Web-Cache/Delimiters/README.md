# Web Cache Delimiter Research

## Overview

Web cache behavior can differ from origin-server behavior when URLs are
parsed, normalized, decoded, or interpreted differently.

These differences can create opportunities for web cache deception
and related cache-related security issues.

## Research Objective

The objective of this research area is to understand how different
components process URL paths and delimiters.

Important areas to examine include:

- URL parsing differences
- Percent-encoding and decoding
- Path normalization
- Cache key construction
- Origin-server path interpretation
- Differences between proxy, cache, and application behavior

## Testing Approach

1. Identify an authorized application and a suitable test endpoint.
2. Understand how the application normally handles the URL.
3. Observe how the cache handles the same request.
4. Compare cache and origin-server responses.
5. Check whether URL normalization or parsing differences affect
   cache behavior.
6. Verify whether any difference produces a real security impact.

## Important Observations

A different response or cache status alone does not establish a
vulnerability.

Confirm whether sensitive or user-specific content can actually be
exposed, cached, or served incorrectly.

## Responsible Testing

Only perform these tests against systems you own or are explicitly
authorized to assess. Avoid actions that could expose other users'
data or disrupt application availability.

## Status

Research documentation started. Additional independently developed
testing resources will be added after validation.
