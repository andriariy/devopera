---
title: New details view in the network panel on stable
authors:
- daniel-herzog
tags:
- dragonfly
license: cc-by-3.0
layout: post
---
Yesterday we released a new version of the Network Logger, with improvements in the way network request details are displayed. Details for each request can now be opened in a resizable overlay, with a dedicated option to wrap long lines. <br/><br/>The details view will now also show the raw headers, rather than just those headers that were parsed and understood by Opera. Generally, there shouldn&#39;t be a difference between raw headers and parsed headers – but one recent example of where you may see some discrepancies are <a href="http://en.wikipedia.org/wiki/SPDY" target="_blank">SPDY</a> requests, which don&#39;t actually have raw headers in the traditional sense. This can be easily observed by checking the network traffic generated when going to sites like <a href="http://isspdyenabled.com/" target="_blank">isspdyenabled.com</a>.<br/><br/><img src="/blog/new-details-view-in-network-panel-on-stable/spdy.png" alt="Opera Dragonfly&#39;s improved Network panel, showing network request details for SPDY traffic." /><br/><br/>In addition, the new &quot;parsed mode&quot; in the nework request details overlay reformats certain POST requests into a more user-friendly layout. In particular, the body of form encoded requests will be shown as name-value pairs, compared to the raw string that is actually sent.<br/><br/><img src="/blog/new-details-view-in-network-panel-on-stable/name-value.png" alt="The new &#39;parsed mode&#39; in the network request details overlay, showing the body of a form encoded POST request as a nice name-value pair table." />
