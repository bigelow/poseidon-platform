# Services Overview

The Poseidon Platform consists of seven specialized microservices, each designed with specific responsibilities and clear boundaries.

## Service Architecture

The platform follows a modular monorepo pattern where each service is:

- **Completely independent**: No runtime dependencies between services
- **Plug-and-play**: Services can be added, removed, or replaced without affecting others
- **Standardized tooling**: Consistent development and deployment patterns
- **Self-contained**: Each service includes all necessary configuration and dependencies

## Core Services

### poseidon-current
**Development Workflows**

- Automated TDD with file watching and instant feedback
- Internal AI-powered commit message generation (local LLM, no external API calls)
- Security-integrated development with SAST scanning
- Professional CLI with natural language commands
- **Status**: ✅ Production Ready (89 tests, 100% coverage, internal AI integration)

### poseidon-forge
**CI/CD Pipelines**

- TDD-integrated build pipelines with comprehensive testing
- Internal AI assistance for pipeline optimization and error analysis
- Security-first pipelines with SAST/DAST integration
- Quality gates and automated testing workflows
- **Status**: 🚧 In Development

### poseidon-harbor
**Deployment Automation**

- Test-validated deployment strategies
- Internal AI-driven deployment optimization and anomaly detection
- Secure deployment with vulnerability scanning
- Zero-downtime deployment strategies
- **Status**: 📋 Planned

### poseidon-lighthouse
**Monitoring & Observability**

- Test coverage monitoring and quality metrics
- Internal AI models for intelligent alerting and root cause analysis
- Security event monitoring and threat detection
- Multi-dimensional metrics collection
- **Status**: 📋 Planned

### poseidon-anchor
**Configuration & Secrets**

- Test-driven configuration management
- Internal AI validation of configuration patterns and security policies
- Secure configuration with encryption at rest
- HashiCorp Vault integration
- **Status**: 📋 Planned

### poseidon-depths
**Infrastructure & Discovery**

- Test-driven infrastructure as code
- Internal AI optimization of resource allocation and service topology
- Secure service discovery with mTLS
- Service discovery with Consul
- **Status**: 📋 Planned

### poseidon-tide
**Data Ingestion Workflows**

- Test-driven data pipeline development
- Internal AI models for data quality validation and pipeline optimization
- Secure data pipeline management with encryption in transit
- Real-time and batch processing
- **Status**: 📋 Planned

## Development Standards

Every service implements these mandatory standards:

- **Dockerfile**: Multi-stage builds with security scanning
- **compose.yml**: Local development environment
- **Taskfile.yml**: Standardized automation tasks
- **requirements.txt**: Dependency management with uv
- **Testing**: Minimum 80% coverage with automated execution
- **Security**: SAST scanning integrated into development workflow
- **Documentation**: Service-specific docs following platform patterns
