# bURL - A pure Bash HTTP client

**Caveat: this is a toy project, not meant to be used for serious purposes. The code is trivial and ugly – is anything else possible when written in shell script? – and probably buggy.**

## Usage

```
Usage: ./burl [options] URL

Options:
  -h            display usage help
  -i            include the HTTP header in the output
  -p <port>     use alternative port number (default: 80)

```

```
$ burl http://tools.ietf.org/html/rfc2616
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
<head profile="http://dublincore.org/documents/2008/08/04/dc-html/">
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <meta name="robots" content="index,follow" />
    <meta name="creator" content="rfcmarkup version 1.115" />
    <link rel="schema.DC" href="http://purl.org/dc/elements/1.1/" />
<meta name="DC.Relation.Replaces" content="rfc2068" />
<meta name="DC.Identifier" content="urn:ietf:rfc:2616" />
<meta name="DC.Date.Issued" content="June, 1999" />
<meta name="DC.Creator" content="Leach, Paul J." />
<meta name="DC.Creator" content="Berners-Lee, Tim" />
<meta name="DC.Creator" content="Mogul, Jeffrey C." />
<meta name="DC.Creator" content="Masinter, Larry" />
<meta name="DC.Creator" content="Fielding, Roy T." />
<meta name="DC.Creator" content="Gettys, James" />
<meta name="DC.Description.Abstract" content="HTTP has been in use by the World-Wide Web global information
initiative since 1990. This specification defines the protocol
referred to as &quot;HTTP/1.1&quot;, and is an update to RFC 2068. [STANDARDS-
TRACK]" />
<meta name="DC.Title" content="Hypertext Transfer Protocol -- HTTP/1.1" />

    <link rel="icon" href="/images/rfc.png" type="image/png" />
    <link rel="shortcut icon" href="/images/rfc.png" type="image/png" />
    <title>RFC 2616 - Hypertext Transfer Protocol -- HTTP/1.1</title>
...
```

## Limitations

Basically, everything beyond fetching a HTTP – no HTTPS, obviously – resource accessible without redirection and with authentication.
