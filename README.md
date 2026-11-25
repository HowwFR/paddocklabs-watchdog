# paddocklabs-watchdog

Checks the PaddockLabs server every 5 minutes. If it stays down for 90 seconds, it restarts it (or un-pauses it) at
most once every 30 minutes, and opens an issue saying what happened and whether it came back.

- Run it by hand: Actions, watchdog, Run workflow. Tick "Test run" to check the whole path without restarting anything.
- Secrets: `SUPABASE_ACCESS_TOKEN` (Supabase account access token) and `SUPABASE_ANON_KEY` (the app's public key).
