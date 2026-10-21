# Dativue for Claude

Research markets, customers, and competitors in Claude using current search data and public social sources.
Dativue combines 20 workflow skills with an authenticated remote MCP connector that exposes 24 research tools.
Results include source links, available provider metrics, and credit accounting so you can distinguish measured evidence from an assistant's interpretation.

## Requirements

- A paid Claude plan that supports plugins, with workspace permission to install a plugin and add its connector
- A Dativue account with enough credits for the research you request
- Internet access to `https://dativue.com/mcp`

The plugin uses a hosted HTTPS server.
It does not require Node.js, Python, an API key, a local MCP process, or social-network credentials.

## Install and connect

1. In Claude, open **Customize > Plugins > Add plugin > Upload plugin** and select `dativue-claude.zip`.
2. Open **Dativue > Connectors** and add the Dativue connector.
   In a team workspace, an owner may need to make it available to the team first.
3. Select **Connect**, sign in to your Dativue account, and approve the `research:read` scope.
4. Open a fresh conversation and enable the Dativue connector if needed.
5. Verify access with the free prompt below before starting paid research.

```text
Use Dativue research_credit_quote to quote one standard keyword_ideas request.
Show the estimated maximum hold and available credits.
Do not run the search.
```

After a directory listing is published, you can install from that listing instead of uploading a ZIP.
Plugin availability and administrator controls can differ by Claude plan and client.
Claude's plugin system supports Chat, Cowork, and Claude Code; each client must expose the connected tools before you can use them there.

For a local Claude Code package check, launch `claude --plugin-dir /absolute/path/to/this/plugin` and complete MCP authentication when prompted.
Do not add a second connector if the existing Dativue connector already points to the same server.

## Try it

```text
Use Dativue to find keyword opportunities for "project management software"
in the United States in English.
Use one basic keyword search only and no more than 4 credits.
Show five relevant keywords with available volume, difficulty, and intent.
Label missing metrics N/A and distinguish data from your recommendations.
```

Other workflows cover Google results and trends, competitor search visibility, backlinks, public social posts and comments, video transcripts, reviews, apps, products, local businesses, website intelligence, technical audits, AI visibility, and product opportunity research.
See [starter prompts](prompts/starter-prompts.md) for examples.
Provider coverage and source availability vary.

## Credits and permissions

Quotes and job-status polling do not charge research credits.
Paid retrievals use the connected Dativue account's credits.
Search may reserve a maximum hold and return unused credits after the provider reports its final cost.
Ask for a quote whenever you need one; routine research can otherwise run directly.
The skills require approval before any individual call whose maximum hold exceeds 50 credits, and an explicit smaller budget in your prompt takes precedence.
The connector does not authorize payment-card charges or account administration.

The tools retrieve public data and cannot post, message, edit, or delete source content.
Research can save results, queue jobs, and change your Dativue credit balance.
Only request public sources and resources you are authorized to use.

## Data handling and support

Claude sends the requested tool inputs to Dativue over HTTPS.
Dativue uses Cloudflare to operate the service, DataForSEO for search research, and Apify and selected actors for public social retrieval.
Relevant queries and public URLs are sent to the provider needed for that request.
Results and credit information return to your Claude conversation.
Do not include passwords, session cookies, API tokens, or private customer data in research prompts.

Full normalized research results and purchased cursor pages are normally deleted within seven days.
Account, security, billing, and ledger records follow the retention described in the privacy policy.
Disconnect the connector in Claude or revoke its access in Dativue when you no longer need it.

- Website and account: [dativue.com](https://dativue.com)
- Privacy: [Privacy policy](https://dativue.com/privacy)
- Terms: [Terms of service](https://dativue.com/terms)
- Help: [Support](https://dativue.com/support) or [team@dativue.com](mailto:team@dativue.com)

Published by Tetriz s.r.o.
The package is proprietary (`UNLICENSED`); access to the Dativue service is subject to its terms.
