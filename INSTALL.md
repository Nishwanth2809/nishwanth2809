# Targeted README fixes

1. Remove the two <img> lines containing `hits.sh/github.com/Nishwanth2809` and `img.shields.io/github/followers/Nishwanth2809`. Keep the status badge.
2. Replace the entire existing `Currently Building` block with FEATURED_PROJECTS.md.
3. Replace the entire existing `GitHub Command Center` block with GITHUB_COMMAND_CENTER.md.
4. Upload both .github/workflows YAML files at the same paths in the GitHub profile repository.
5. Create an Actions secret named `SUMMARY_GITHUB_TOKEN`, containing a GitHub personal access token with sufficient read access to your account statistics and repository permissions to write generated images. Do not paste secrets into files.
6. In repo Settings > Actions > General, allow workflows read and write permissions if needed.
7. Run `GitHub Profile Summary` and `Update Activity Graph` once manually in Actions. Images will not exist until successful runs.
8. Keep the existing snake section as-is.

Notes: The GitHub stats services previously used can fail due to rate limits. The summary action needs a personal access token; the activity graph uses the repository GITHUB_TOKEN. GitHub Actions may require workflow approval or appropriate permissions.
