# Waku Roadmap 2024 Gantt Charts

The aim of those charts is to provide a visual on the 2024 milestones, contributor work and completion dates.
In **red** are the critical path for Status app short term goals.

**Note the contributor assignments may not exactly match reality.**
**This is still a draft.**

```mermaid
gantt
    title Waku 2024
    dateFormat YYYY-MM-DD
    axisFormat %d-%b

    section Status - Basic Reliability
        Enable testing of direct messages: crit, milestone, after test-direct-msg, 0
        Review connection management: crit, milestone, 0
    section Validate RLN Relay
        Store v3-beta (msg hash): crit, milestone, after storev3-br storev3-bn storev3-bj storev3-bg, 0
        Store v3 (sync): crit, milestone, after storev3r storev3n storev3j, 0 
        PostgreSQL maintenance: crit, milestone, after pgsql, 0
        RLNv2 in nwaku: milestone, after rlnv2, 0
        Maturing RLN: milestone, after maturing-rln, 0
        Reliability Protocol for Relay: crit, milestone, after relrelay, 0
        NodeJS SDK: milestone, after nodejs, 0
    section Service Consumer Validation
        DoS protection for req-res protocols: crit, milestone, after dosreqresn dosreqresj dosreqresg, 0
        Provision RLN for light push clients PoC: milestone, after provisionrlnr provisionrlnj, 0
        Reliability Protocol for Resource-Restricted Clients: crit, milestone, after relresreqc relresreqj, 0
        Local Web Development: milestone, after localweb, 0
        React Native: milestone, after reactnative, 0
    section Service Incentization
        Service incentivisation (first PoC): milestone, after i18npoc1r, 0
        Service incentivisation (second PoC): milestone, after i18npoc2r, 0
        Roadmap Towards Incentivisation on Mainnet: milestone, after i18nmainnetr, 0
        Active Capability Service Discovery PoC: milestone, after csdr, 0
    section chat - plopezlpz
        todo: todo, 2024-01-01, 1d
    section richard-ramos
        Store v3-beta (go-waku): crit, storev3-bg, after storev3-br, 3w
    section chaitanyaprem
        Store v3 (sync): crit, 2024-02-08, 2024-04-26
        DoS protection for req-res protocols: crit, dosreqresg, after dosreqresn, 15d
        Reliability Protocol for Resource-Restricted Clients: crit, relresreqc, after dosreqresg, 21d
    section research
    section research - jm-clius
        White Paper: whitepaper, 2024-01-01, 360d
        RFC review: rfc-review, 2024-01-01, 90d
    section research - alrevuelta
        RLN in resource-restricted clients: rlnrestricted, 2024-01-01, 110d
        RLNv2: rlnv2, 2024-01-01, 120d
        Maturing RLN: maturing-rln, 2024-01-01, 360d
    section research - sionois
        Store v3-beta (msg hash): crit, storev3-br, 2024-01-01, 120d
        Store v3 (sync): crit, storev3r, after storev3-br, 120d
        Active Capability Service Discovery PoC: csdr, after storev3r, 90d
    section research - s-tikhomirov
        Incentivization PoC 1: i18npoc1r, 2024-01-01, 20w
        Incentivization PoC 2: i18npoc2r, after i18npoc1, 120d
        Incentivization Mainnet Roadmap: i18nmainnetr, after i18npoc1, 240d
    section research - shash256
        Provision RLN for light push clients PoC: provisionrlnr, 2024-04-28, 30d
    section nwaku - ivansete
        PostgreSQL Maintenance: crit, pgqsl, 2024-01-01, 90d
        Store v3-beta (hardening): crit, storev3-bn, after storev3-br, 3w
        Store v3 (hardening): crit, storev3n, after storev3r, 3w
        NodeJS SDK: nodejs, 2024-03-01, 120d
    section nwaku - NagyZoltanPeter
        DoS Protection for Req-Res Protocols: crit, dosreqresn, 2024-01-01, 90d
    section nwaku - gabrielmer
        Reliability Protocol for Relay: crit, relrelay, 2024-05-01, 90d
        Ethereum Address to Secure Channel: ethadr, 2024-09-01, 3w
    section nwaku - new hire 1
        FQDN-Less Browser Connections: webrtcn, 2024-09-01, 3w
        WebTransport: webtransportn, after webrtcn, 5w
    section js-waku - weboko
        RLN in resource-restricted clients: rlnlight, 2024-01-01, 90d
        Local Web Development: localweb, 2024-02-01, 30d
        React Native: reactnative, 2024-03-01, 30d
        DoS Protection for Req-Res Protocols: crit, dosreqresj, after dosreqresn, 30d
        Provision RLN for light push clients PoC: provisionrlnj, after dosreqresj, 15d
    section js-waku - danisharora099
        Reliability for Req-Res Protocols: crit, relreqresj, 2024-01-01, 90d
        Incentivization PoC 1: i18npoc1j, after i18npocr, 120d
    section js-waku - adklempner
        Auto-sharding and static sharding: crit, shard, 2024-01-01, 90d
        RLN in resource-restricted clients: rlnlight, 2024-01-01, 90d
        Store v3-beta (msg hash): crit, storev3-bj, after storev3-br, 90d
    section js-waku - new hire 1
        FQDN-Less Browser Connections: webrtcj, 2024-06-01, 45d
        WebTransport: webtransportj, after webtransportn, 30d
```
