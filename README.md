# Install dependencies
mix deps.get

# Prepare ENV
export GH_TOKEN=

# Dry run, without committing
mix run -e "ProfileUpdater.run(true)"
cat output.md

# Real run
mix run -e "ProfileUpdater.run"
