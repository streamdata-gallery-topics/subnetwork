swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 1
info:
  title: AWS Route 53 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /2013-04-01/testdnsanswer&amp;edns0clientsubnetip=EDNS0ClientSubnetIP&amp;edns0clientsubnetmask=EDNS0ClientSubnetMask?hostedzoneid=HostedZoneId&amp;recordname=RecordName&amp;recordtype=RecordType&amp;resolverip=ResolverIP
  : get:
      summary: Test D N S Answer
      description: Gets the value that Amazon Route 53 returns in response to a DNS
        request for a specified record name and type. You can optionally specify the
        IP address of a DNS resolver, an EDNS0 client subnet IP address, and a subnet
        mask.
      operationId: testdnsanswer
      x-api-path-slug: 20130401testdnsanswerampedns0clientsubnetipedns0clientsubnetipampedns0clientsubnetmaskedns0clientsubnetmaskhostedzoneidhostedzoneidamprecordnamerecordnameamprecordtyperecordtypeampresolveripresolverip-get
      parameters:
      - in: path
        name: edns0clientsubnetip
        description: If the resolver that you specified for resolverip supports EDNS0,
          specify the IP address of a client in the applicable location
        type: string
      responses:
        200:
          description: OK
      tags:
      - DNS