# GraphQL qieries used by the CI

## Queries to the node's regular GraphQL server

- `query { daemonStatus }`
- `query { bestChain }`
- `query { block }`
 
## Detailed Queries

- `query {bestChain(maxLength: 5) {protocolState {consensusState {blockHeight}} stateHash}}`
- `query {bestChain(maxLength: 1) {stateHash}}`
- `query {block(stateHash: "$hash") {stateHash}}`
- `query {daemonStatus { highestBlockLengthReceived }}`
- `query {bestChain(maxLength: 1) {protocolState {consensusState {blockHeight}}}}`
- `query {bestChain(maxLength: 1) {protocolState {consensusState {blockHeight}}}}`
- `query {bestChain(maxLength: 1) {protocolState {consensusState {epoch}}}}`
- `query {bestChain(maxLength: 1) {protocolState {consensusState {slot}}}}`
- `query {bestChain(maxLength: 1) {protocolState {consensusState {epoch slot}}}}`
