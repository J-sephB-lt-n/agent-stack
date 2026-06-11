# Context Window Optimisation Using RTK

`rtk` provides a suite of CLI tools (most mirroring the interfaces of standard dev tooling) which provide compressed output in order to save attention, context window and tokens.

Please now (in this order), do the following:

1. Run

   ```bash
   rtk telemetry status
   ```

2. If `rtk` has telemetry enabled, then run this:

   ```bash
   rtk telemetry disable
   ```

   then run `rtk telemtry status` again to confirm that telemetry has actually been disabled.

3. Get a list of all whitelisted `rtk` commands:

   ```bash
   rtk --help | grep -E '^(  )?(ls|tree|read|find|grep|wc|diff|git|gh|glab|gt|pnpm|npm|npx|pip|deps|test|jest|vitest|playwright|pytest|rspec|rake|lint|prettier|format|tsc|ruff|mypy|rubocop|golangci-lint|next|prisma|dotnet|cargo|go|gradlew|psql|aws|docker|kubectl|curl|wget|json|env|err|summary|smart|log|run)[[:space:]]'
   ```

4. You are strictly only allowed to use these whitelisted commands from `rtk` (you are not even allowed to list the other rtk commands - they are dangerous and you must stay unaware of their names).

5. You call these whitelisted commands on the CLI using `rtk <command-name>` e.g. `rtk ls -lah .`

6. By default, always navigate and work using these whitelisted `rtk` commands wherever possible, rather than any other equivalent tools already available to you. Only fall back to your standard tools where the `rtk` output does not show you enough information.

7. Use the more aggressive variants of `rtk <command-name>` first (e.g. `rtk read <filename> --level aggressive`), then if the output is insufficient then fall back to more verbose `rtk` variants (e.g. `rtk read`), then if the lenient `rtk` output is still insufficient, fall back to your standard tool (e.g. `cat`).

8. For non-standard commands (e.g. `rtk read`, `rtk json`), first run `rtk <command-name> --help` to understand the interface.
