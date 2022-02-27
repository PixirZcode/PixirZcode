# Install dependencies
mix deps.get

# Prepare ENV
export GH_TOKEN=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

# Dry run, without committing
mix run -e "ProfileUpdater.run(true)"
cat output.md

# Real run
mix run -e "ProfileUpdater.run"
