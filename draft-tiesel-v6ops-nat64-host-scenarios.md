---
title: Application Scenarios for NAT64 from Host Perspective
abbrev: draft-tiesel-v6ops-nat64-host-scenarios
category: info

docname: draft-tiesel-v6ops-nat64-host-scenarios
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
# area: Operations and Management Area
# workgroup: IPv6 Operations
keyword:
  - IPv6
  - transition technologies
  - CLAT
  - 464XLAT
  - DNS
  - DNS64
  - APIs

venue:
#  group: v6ops
#  type: Working Group
#  mail: v6ops@ietf.org
#  arch: https://mailarchive.ietf.org/arch/browse/v6ops/
  github: "philsbln/v6ops-host-based-tt"
  latest: "https://philsbln.github.io/v6ops-host-based-tt/draft-tiesel-v6ops-nat64-host-scenarios.html"

author:
 -
    fullname: Philipp S. Tiesel
    organization: SAP SE
    email: philipp@tiesel.net

normative:

informative:


--- abstract

This document gives an overview about about application scenarios using NAT64 from a host perspective enabling applications on these hosts to reach the IPv4 Internet using NAT64.
It describes the operational aspects of using of CLAT, DNS64, and host based address synthesis. 

--- middle

# Introduction

Stateful NAT64 {{?RFC6146}}, a mechanism for translating IPv6 packets to IPv4 packets and vice versa,
is crucial for IPv6 only hosts to reach endpoints that are not reachable using IPv6 yet.
In order for hosts to open a connection to an IPv4 endpoint facilitating NAT64,
the IPv4 destination address first needs to be used to synthesize an IPv6 address that embeds the IPv4 address so that NAT64 can extract it.
This document describes from a host's perspective how this synthesis can be achieved using CLAT, DNS64, and address synthesis within the host's resolver stack or network API.

# Conventions and Definitions

{::boilerplate bcp14-tagged}


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
