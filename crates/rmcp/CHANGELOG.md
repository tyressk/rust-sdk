# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.1](https://github.com/modelcontextprotocol/rust-sdk/compare/rmcp-v0.2.0...rmcp-v0.2.1) - 2025-07-03

### Other

- *(docs)* Minor README updates ([#301](https://github.com/modelcontextprotocol/rust-sdk/pull/301))

## [0.2.0](https://github.com/modelcontextprotocol/rust-sdk/compare/rmcp-v0.1.5...rmcp-v0.2.0) - 2025-07-02

### Added

- mark boxed http body as sync ([#291](https://github.com/modelcontextprotocol/rust-sdk/pull/291))
- add progress notification handling and related structures ([#282](https://github.com/modelcontextprotocol/rust-sdk/pull/282))
- allow failable service creation in streamable HTTP tower service ([#244](https://github.com/modelcontextprotocol/rust-sdk/pull/244))
- provide more context information ([#236](https://github.com/modelcontextprotocol/rust-sdk/pull/236))
- stateless mode of streamable http client ([#233](https://github.com/modelcontextprotocol/rust-sdk/pull/233))
- add cancellation_token method to `RunningService` ([#218](https://github.com/modelcontextprotocol/rust-sdk/pull/218))
- better http server support ([#199](https://github.com/modelcontextprotocol/rust-sdk/pull/199))
- throw initialize error detail ([#192](https://github.com/modelcontextprotocol/rust-sdk/pull/192))
- sse client optionally skip the endpoint event ([#187](https://github.com/modelcontextprotocol/rust-sdk/pull/187))
- *(server)* add annotation to tool macro ([#184](https://github.com/modelcontextprotocol/rust-sdk/pull/184))
- *(model)* add json schema generation support for all model types ([#176](https://github.com/modelcontextprotocol/rust-sdk/pull/176))
- *(openapi)* add OpenAPI v3 compatibility and test for nullable field schema workaround ([#135](https://github.com/modelcontextprotocol/rust-sdk/pull/135)) ([#137](https://github.com/modelcontextprotocol/rust-sdk/pull/137))
- *(extension)* extract http request part into rmcp extension ([#163](https://github.com/modelcontextprotocol/rust-sdk/pull/163))
- *(transport)* support streamable http server ([#152](https://github.com/modelcontextprotocol/rust-sdk/pull/152))
- *(oauth)* fixes + cache client credentials ([#157](https://github.com/modelcontextprotocol/rust-sdk/pull/157))
- allow use of reqwest without ring provider ([#155](https://github.com/modelcontextprotocol/rust-sdk/pull/155))
- extensions to context ([#102](https://github.com/modelcontextprotocol/rust-sdk/pull/102))
- revision-2025-03-26 without streamable http ([#84](https://github.com/modelcontextprotocol/rust-sdk/pull/84))
- *(tool)* allow tool call return a serializable value in json format ([#75](https://github.com/modelcontextprotocol/rust-sdk/pull/75)) ([#78](https://github.com/modelcontextprotocol/rust-sdk/pull/78))
- Sse server auto ping ([#74](https://github.com/modelcontextprotocol/rust-sdk/pull/74))
- *(transport)* Sse client transport trait ([#67](https://github.com/modelcontextprotocol/rust-sdk/pull/67))

### Fixed

- let users decide what to wrap in child process command ([#279](https://github.com/modelcontextprotocol/rust-sdk/pull/279))
- cancellable initialization process ([#280](https://github.com/modelcontextprotocol/rust-sdk/pull/280))
- inject part into extension when handing init req ([#275](https://github.com/modelcontextprotocol/rust-sdk/pull/275))
- streamable http server close request channel on response([#266](https://github.com/modelcontextprotocol/rust-sdk/pull/266)) ([#270](https://github.com/modelcontextprotocol/rust-sdk/pull/270))
- streamable http client close on response ([#268](https://github.com/modelcontextprotocol/rust-sdk/pull/268))
- expose TokioChildWrapper::id() in TokioChildProcess and TokioChildProcessOut ([#254](https://github.com/modelcontextprotocol/rust-sdk/pull/254))
- add compatibility handling for non-standard notifications in async_rw ([#247](https://github.com/modelcontextprotocol/rust-sdk/pull/247))
- allow SSE server router to be nested ([#240](https://github.com/modelcontextprotocol/rust-sdk/pull/240))
- error for status in post method of streamable http client ([#238](https://github.com/modelcontextprotocol/rust-sdk/pull/238))
- disable wasmbind in chrono for wasm32-unknown-unknown ([#234](https://github.com/modelcontextprotocol/rust-sdk/pull/234))
- *(examples)* add clients in examples's readme ([#225](https://github.com/modelcontextprotocol/rust-sdk/pull/225))
- generic ServerHandler ([#223](https://github.com/modelcontextprotocol/rust-sdk/pull/223))
- comment error ([#215](https://github.com/modelcontextprotocol/rust-sdk/pull/215))
- resolve the server 406 error in API calls ([#203](https://github.com/modelcontextprotocol/rust-sdk/pull/203))
- sse endpoint build follow js's `new URL(url, base)` ([#197](https://github.com/modelcontextprotocol/rust-sdk/pull/197))
- more friendly interface to get service error ([#190](https://github.com/modelcontextprotocol/rust-sdk/pull/190))
- cleanup zombie processes for child process client ([#156](https://github.com/modelcontextprotocol/rust-sdk/pull/156))
- *(schemar)* use self-defined settings ([#180](https://github.com/modelcontextprotocol/rust-sdk/pull/180))
- *(transport-sse-server)* cleanup on connection drop ([#165](https://github.com/modelcontextprotocol/rust-sdk/pull/165))
- *(test)* skip serialize tool's annotation if empty ([#160](https://github.com/modelcontextprotocol/rust-sdk/pull/160))
- fix resource leak ([#136](https://github.com/modelcontextprotocol/rust-sdk/pull/136))
- *(handler)* do call handler methods when initialize server ([#118](https://github.com/modelcontextprotocol/rust-sdk/pull/118))
- *(server)* schemars compilation errors ([#104](https://github.com/modelcontextprotocol/rust-sdk/pull/104))
- *(test)* fix test introduced by #97 ([#101](https://github.com/modelcontextprotocol/rust-sdk/pull/101))
- *(macro)* add generics marco types support ([#98](https://github.com/modelcontextprotocol/rust-sdk/pull/98))
- *(typo)* nit language corrections ([#90](https://github.com/modelcontextprotocol/rust-sdk/pull/90))
- *(typo)* s/marcos/macros/ ([#85](https://github.com/modelcontextprotocol/rust-sdk/pull/85))
- *(client)* add error enum while deal client info ([#76](https://github.com/modelcontextprotocol/rust-sdk/pull/76))
- *(notification)* fix wrongly error report in notification ([#70](https://github.com/modelcontextprotocol/rust-sdk/pull/70))
- *(test)* fix tool deserialization error ([#68](https://github.com/modelcontextprotocol/rust-sdk/pull/68))
- *(server)* add error enum while deal server info ([#51](https://github.com/modelcontextprotocol/rust-sdk/pull/51))

### Other

- add simpling example and test ([#289](https://github.com/modelcontextprotocol/rust-sdk/pull/289))
- add update for test_message_schema ([#286](https://github.com/modelcontextprotocol/rust-sdk/pull/286))
- add notion clear in model.rs ([#284](https://github.com/modelcontextprotocol/rust-sdk/pull/284))
- cov settings, and fix several building warnings ([#281](https://github.com/modelcontextprotocol/rust-sdk/pull/281))
- refactor tool macros and router implementation ([#261](https://github.com/modelcontextprotocol/rust-sdk/pull/261))
- fix regression in URL joining ([#265](https://github.com/modelcontextprotocol/rust-sdk/pull/265))
- remove erroneous definitions_path  ([#264](https://github.com/modelcontextprotocol/rust-sdk/pull/264))
- allow using a TokioCommandWrap for TokioChildProcess::new closes #243 ([#245](https://github.com/modelcontextprotocol/rust-sdk/pull/245))
- Fix typo ([#249](https://github.com/modelcontextprotocol/rust-sdk/pull/249))
- provide http server as tower service ([#228](https://github.com/modelcontextprotocol/rust-sdk/pull/228))
- *(deps)* update sse-stream requirement from 0.1.4 to 0.2.0 ([#230](https://github.com/modelcontextprotocol/rust-sdk/pull/230))
- Server info is only retrieved once during initialization ([#214](https://github.com/modelcontextprotocol/rust-sdk/pull/214))
- *(deps)* update base64 requirement from 0.21 to 0.22 ([#209](https://github.com/modelcontextprotocol/rust-sdk/pull/209))
- revert badge ([#202](https://github.com/modelcontextprotocol/rust-sdk/pull/202))
- use hierarchical readme for publishing ([#198](https://github.com/modelcontextprotocol/rust-sdk/pull/198))
- Ci/coverage badge ([#191](https://github.com/modelcontextprotocol/rust-sdk/pull/191))
- fix error introduced by merge, and reorganize feature ([#185](https://github.com/modelcontextprotocol/rust-sdk/pull/185))
- Transport trait and worker transport, and streamable http client with those new features. ([#167](https://github.com/modelcontextprotocol/rust-sdk/pull/167))
- add oauth2 support ([#130](https://github.com/modelcontextprotocol/rust-sdk/pull/130))
- remove un-used tower.rs ([#125](https://github.com/modelcontextprotocol/rust-sdk/pull/125))
- update calculator example description ([#115](https://github.com/modelcontextprotocol/rust-sdk/pull/115))
- fix the url ([#120](https://github.com/modelcontextprotocol/rust-sdk/pull/120))
- add a simple chat client for example ([#119](https://github.com/modelcontextprotocol/rust-sdk/pull/119))
- add an overview to `rmcp/src/lib.rs` ([#116](https://github.com/modelcontextprotocol/rust-sdk/pull/116))
- *(context)* test context request handling and refactor for reusable client-server tests ([#97](https://github.com/modelcontextprotocol/rust-sdk/pull/97))
- *(logging)* Add tests for logging  ([#96](https://github.com/modelcontextprotocol/rust-sdk/pull/96))
- Adopt Devcontainer for Development Environment ([#81](https://github.com/modelcontextprotocol/rust-sdk/pull/81))
- fix typos ([#79](https://github.com/modelcontextprotocol/rust-sdk/pull/79))
- format and fix typo ([#72](https://github.com/modelcontextprotocol/rust-sdk/pull/72))
- add documentation generation job ([#59](https://github.com/modelcontextprotocol/rust-sdk/pull/59))
- add test with js server ([#65](https://github.com/modelcontextprotocol/rust-sdk/pull/65))
- fmt the project ([#54](https://github.com/modelcontextprotocol/rust-sdk/pull/54))
- *(sse_server)* separate router and server startup ([#52](https://github.com/modelcontextprotocol/rust-sdk/pull/52))
- fix broken link ([#53](https://github.com/modelcontextprotocol/rust-sdk/pull/53))
- fix the branch name for git dependency ([#46](https://github.com/modelcontextprotocol/rust-sdk/pull/46))
- Move whole rmcp crate to official rust sdk ([#44](https://github.com/modelcontextprotocol/rust-sdk/pull/44))
- Initial commit
