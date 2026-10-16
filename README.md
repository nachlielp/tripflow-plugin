# TripFlow for Claude

A Claude Code plugin marketplace for [TripFlow](https://tripflow.cc), the
collaborative, map-first trip planner. The `tripflow` plugin connects Claude to
your TripFlow account. You can list and inspect trips, create new ones, search
Google Places, add or edit dated and saved places, and review recent trip
activity.

## Install

```
/plugin install tripflow --marketplace nachlielp/tripflow-plugin
```

Or add the marketplace first, then install:

```
/plugin marketplace add nachlielp/tripflow-plugin
/plugin install tripflow@tripflow
```

Then run `/mcp`, choose `plugin:tripflow:tripflow`, and sign in with your
TripFlow account. Sign-in opens your browser and returns to
`http://localhost:8080/callback`, so port 8080 must be free at that moment. If a
tool reports a missing profile, finish setup at https://tripflow.cc/connect.

## What's included

- **MCP server:** `https://tripflow.cc/mcp` (Streamable HTTP, OAuth with PKCE;
  no secrets are bundled).
- **Skill:** `plan-trip` tells Claude to read a trip before editing it, ask when
  search results are ambiguous, and confirm before deleting a place.

The plugin can't book or pay for travel, delete whole trips, manage trip
members, reorder stops, calculate routes, or upload photos. Use the web app at
https://tripflow.cc for those.

## Links

- Website: https://tripflow.cc
- Support: https://tripflow.cc/support
- Privacy: https://tripflow.cc/privacy
- Terms: https://tripflow.cc/terms
