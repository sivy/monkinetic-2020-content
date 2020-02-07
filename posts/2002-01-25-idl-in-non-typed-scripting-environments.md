date: 2002-01-25
slug: idl-in-non-typed-scripting-environments
title: IDL in non-typed scripting environments
---
Dave is [making a point](http://scriptingnews.userland.com/backissues/2002/01/24#l1eb33a91f4a7ab582451d453177a6603) on Scripting News regarding IDL (or in this case WSDL) for Frontier, and other non-typed scripting languages. His point is that he cannot generate at runtime the WSDL directly from the code, as can C# or Java developers - b/c their runtimes have information about the types and numbers of parameters to a call.

This means having to handcode the WSDL for a web service in these environments, which can be a PITA if your service is at all large.

<img align="right" border="1" hspace="2" src="https://media.redmonk.net/images/idlScript.jpg" vspace="2"/>

I have an idea though. One way to get around this would be to implement a meta-data header for these environments similar to javadoc. I'll use Frontier as an example.

In Frontier, scripts are outlines. Frontier already has a [rich set of functionality](http://docserver.userland.com/op/) dealing with rendering outlines into other formats, esp. [HTML](http://docserver.userland.com/html/). You can use \#directives in your outlines, which get translated into information in the symbol table when rendering the outline (or any other datatype for that matter).

 So, I would propose a simple set of \#directives that can be inserted into a script outline above the actual script code, as a commented block. That block can be grabbed and processed to generate whatever idl format is desired.

This is just an idea, someone with more Frontier experience could come up with a better design. I also know that Perl has [Perldoc](http://www.perldoc.com/) and [POD](http://www.perldoc.com/perl5.6.1/pod.html) (inline support for manpages), so including this information in perl scripts in a long tradition in that community.

Also, at least [someone](http://mail.python.org/pipermail/python-list/2001-June/046402.html) is working on WSDL support in Python (which has an easily introspected runtime). "Therefore I am planning to write a WSDL generator that will examine our exposed methods and write out a valid WSDL file."

So, I think that lack of explicitly typed data should not be the final reason not to support some sort of IDL for web services. There may be other, better reasons, but I have not seen them yet.