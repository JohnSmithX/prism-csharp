# Prism C# sdk

Deps framework 2.0

## Usage:

```
using Prism;

string host = "http://avvtupnm.local:8080/api";
string key = "umjj5xj6";
string secret = "xa4k7gzyemzjkscapdjb";

PrismClient client = new PrismClient(host, key, secret);

PrismParams p = new PrismParams();
p["e"] = "va";
p["c"] = "va";
p["b"] = "vb";
p["0"] = "v0";

PrismResponse rsp = client.Get("platform/notify/status", p);
Console.WriteLine(rsp.RequestId);
Console.WriteLine(rsp);
```

## Todo:

1. oauth login
1. notify