# copilot-documentation-action
A Github Action that updates repository documentation every week.

Requires you have access to the Github Copilot Agent, which currently requires a Github Pro+ or Enterprise subscription.

Requires you setup a PAT with the correct permissions and store it in a secret called `GH_ACTION_PAT`; see https://docs.github.com/en/enterprise-cloud@latest/copilot/how-tos/use-copilot-agents/coding-agent/assign-copilot-to-an-issue#creating-and-assigning-a-new-issue

Update the prompt as needed in the action yaml file. Search/replace `your_org_name` and `your_repo_name` with the correct values.


# Example Output

This comprehensive weekly documentation update addresses all gaps identified in the repository documentation audit. The changes ensure complete accuracy and alignment between documentation and the actual codebase.

### Major Updates

#### 🏗️ Architecture Documentation
- **Added Cloudflare Workers**: Documented the `workers/news-summary/` service which was missing from all architecture overviews
- **Utility Services**: Created comprehensive documentation for `utils/fly-log-shipper/` and `utils/golinks/` services
- **Service Coverage**: Updated main README and docs to reflect 100% of active services and components

#### 🔧 Version Consistency Fixes
- **Python Version**: Updated all references from 3.11 → 3.12 to match `pyproject.toml` configuration
- **Node.js Version**: Updated all references from 18 → 22 to match actual CI workflow files
- **PostgreSQL Version**: Fixed documentation mismatch (docs said 17, `docker-compose.yml` uses 15)

#### 📋 Service Documentation
- **TypeScript Workers**: Updated packages documentation to accurately reflect Temporal workers for user engagement
- **News Processing**: Added comprehensive setup and deployment instructions for Cloudflare Workers
- **CI/CD Coverage**: Enhanced workflow documentation with detailed Cloudflare Workers deployment process

#### 📁 New Documentation
Created `docs/UTILITY_SERVICES.md` covering:
- Log aggregation service configuration and deployment
- GoLinks internal link management system
- Fly.io deployment procedures for utility services
- Monitoring and troubleshooting guidelines

### Configuration Accuracy

All setup instructions, environment variables, and tool versions now match actual configuration files:
- Docker Compose service versions aligned with documentation
- CI/CD workflow examples match actual GitHub Actions files
- Environment setup scripts verified and enhanced with clearer annotations
- Package structure documentation reflects actual implementation

### Quality Improvements

- **Link Validation**: Verified all internal references and external links
- **File Verification**: Confirmed all referenced scripts, configs, and workflows exist
- **Cross-References**: Added navigation links between related documentation files
- **Setup Instructions**: Enhanced with comprehensive coverage for all development scenarios

The documentation now provides accurate, complete coverage of the MarketStreet monorepo architecture and development setup procedures.
