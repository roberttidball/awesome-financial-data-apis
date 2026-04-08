# Contributing to Awesome Financial Data APIs

Thank you for helping maintain this list. The most valuable contributions are **verifications** — confirming that an API still works, or flagging that a previously listed API has broken or changed its terms.

## What We Accept

**High-priority contributions**:
- Status updates (🟢 / 🟡 / 🔴) with verification date and evidence
- New APIs or libraries that are actively maintained and fill a gap in the list
- New code recipes for common data tasks
- Corrections to rate limit information (these change frequently)

**Lower-priority contributions**:
- New sections for new data categories (discuss in an issue first)
- Major structural changes (always open an issue before a PR)

## What We Do Not Accept

- APIs that are not publicly documented (no undocumented scraping tricks)
- Libraries with no activity in the past 24 months (unless explicitly listed as "legacy")
- Paid-only APIs with no trial or free tier without clear disclosure
- Broken links without a replacement or removal
- Promotional content written by the API's own team (disclose your affiliation)

## Verification Standard

Before submitting a new API or updating a status:

1. **Actually call the API** with the listed example code and confirm it works.
2. **Record the verification date** (use YYYY-MM format).
3. **Note the Python version** and key library versions you tested with.

If you cannot verify an entry but believe its status has changed, open an issue rather than a PR.

## Format Guidelines

Follow this format for new API entries:

```markdown
**[API Name](https://api-url.com/)**
- **Free**: Describe the free tier honestly (rate limits, data age, etc.)
- **Data**: What data types are available
- **Python**: `pip install library-name`
- **Note**: Anything important that affects usability

```python
# Minimal working example (copy-paste should work)
import library
client = library.Client(api_key='YOUR_KEY')
data = client.get('AAPL')
```
```

## Affiliation Disclosure

If you work for or are financially affiliated with a company whose API you are adding, disclose this in your PR description. We may still accept the contribution if it meets our quality standards, but disclosure is required.

## Pull Request Process

1. Fork the repository
2. Make your changes in a descriptive branch (`update-polygon-status`, `add-simfin-recipe`)
3. Verify all code examples work
4. Submit a PR with a brief explanation of what changed and why
5. PRs are reviewed within 2 weeks; status-update PRs are fast-tracked

## Reporting Broken Links or APIs

Open a GitHub Issue with:
- The API name and current status
- Evidence the API has broken (error message, HTTP status code, date observed)
- If known: whether this is temporary maintenance or a permanent change

## Code of Conduct

Be accurate, be honest, disclose affiliations. Financial data is a domain where inaccurate information has real consequences for people building investment tools.
