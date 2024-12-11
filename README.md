# Express.js JSON Body Parsing Issue

This repository demonstrates a common issue encountered when working with JSON request bodies in Express.js applications.  The problem arises when the client doesn't send the correct `Content-Type` header, or it's missing altogether. This leads to the `req.body` being empty, causing unexpected behavior.

The `bug.js` file shows the problematic code, while `bugSolution.js` demonstrates the corrected version.

## Problem
The server expects JSON data, but without the header, it won't parse the data correctly, leading to an empty `req.body` object, causing unexpected behavior or errors further down in the request handling chain.  This issue might be difficult to debug since the server shows no error, it just silently doesn't receive the data.