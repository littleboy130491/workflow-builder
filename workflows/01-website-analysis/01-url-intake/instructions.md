# Step 01: URL Intake — Instructions

## Objective

Collect the target website URL and any optional reference sites from the user.

## Process

1. Prompt the user to provide:
   - The full URL of the website they want to redesign
   - (Optional) One or more reference URLs for design inspiration

2. Validate that each URL is properly formatted and accessible

3. Save outputs:
   - Write the website URL to `outputs/01-url-intake/website-url.txt`
   - Write reference URLs to `outputs/01-url-intake/reference-urls.txt` (one per line, or "NONE" if not provided)

## Notes

- If the user provides multiple reference URLs, keep all of them
- If no references are provided, this will be handled in Step 04 (Reference Identification)
- Store URLs exactly as provided (no trailing slashes removed unless user specifies)
