# Data Sources

CTFL can read usage data from multiple sources. Configure this in **Settings → Usage Data Source**.

## Local logs

Reads Claude Code conversation files from `~/.claude/projects/`. This is the default — no API key needed.

Provides:

- Token counts (input/output) per conversation
- Per-project and per-model breakdowns
- Cost estimates (optional, based on public pricing)

## Admin API

Fetches organization-level usage from the [Anthropic Admin API](https://docs.anthropic.com/en/docs/administration/admin-api). Requires an admin API key.

Provides:

- Accurate token counts and costs from Anthropic's billing data
- Organization-wide usage (not just local conversations)

To set up:

1. Go to **Settings → Admin API Key**
2. Enter your Anthropic Admin API key
3. Set data source to **Admin API** or **Both**

## Both

Merges data from local logs and the Admin API. Use this to get the most complete picture — local project breakdowns combined with accurate API billing data.

## OAuth / Rate limits

CTFL also reads your Claude Code OAuth credentials from `~/.claude/.credentials.json` to fetch plan utilization (session and weekly limits) directly from `claude.ai`.

This happens automatically if you're logged into Claude Code — no configuration needed. Token refresh is handled transparently.

The rate limit data appears in:

- The tooltip (if enabled)
- The usage popup's rate limits section
- Desktop notifications when utilization exceeds the configured threshold
