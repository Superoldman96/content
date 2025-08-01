---
title: declarativeNetRequest.MAX_NUMBER_OF_DYNAMIC_AND_SESSION_RULES
slug: Mozilla/Add-ons/WebExtensions/API/declarativeNetRequest/MAX_NUMBER_OF_DYNAMIC_AND_SESSION_RULES
page-type: webextension-api-property
browser-compat: webextensions.api.declarativeNetRequest.MAX_NUMBER_OF_DYNAMIC_AND_SESSION_RULES
sidebar: addonsidebar
---

The maximum number of dynamic and session-scoped rules an extension can add.

- Until Firefox 126, this property had a value of 5,000 and indicated that an extension could create up to 5,000 dynamic rules and up to 5,000 session-scope rules. This property was deprecated in Firefox 126, and the limits are now defined separately for each rule type by {{WebExtAPIRef("declarativeNetRequest.MAX_NUMBER_OF_DYNAMIC_RULES")}} and {{WebExtAPIRef("declarativeNetRequest.MAX_NUMBER_OF_SESSION_RULES")}}.
- Until Chrome 119, this property had a value of 5,000 and indicated that an extension could create any combination of dynamic and session-scope up to 5,000. This property was deprecated in Chrome 120. See [rule limits](https://developer.chrome.com/docs/extensions/reference/api/declarativeNetRequest#limits) in the Chrome documentation for information on limits in Chrome 120 and higher.
- In Safari, this property has a value of 30,000 and indicates an extension can create any combination of dynamic and session-scope rules up to 30,000.

{{WebExtExamples("h2")}}

## Browser compatibility

{{Compat}}

<!--
// Copyright 2015 The Chromium Authors. All rights reserved.
//
// Redistribution and use in source and binary forms, with or without
// modification, are permitted provided that the following conditions are
// met:
//
//    * Redistributions of source code must retain the above copyright
// notice, this list of conditions and the following disclaimer.
//    * Redistributions in binary form must reproduce the above
// copyright notice, this list of conditions and the following disclaimer
// in the documentation and/or other materials provided with the
// distribution.
//    * Neither the name of Google Inc. nor the names of its
// contributors may be used to endorse or promote products derived from
// this software without specific prior written permission.
//
// THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
// "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
// LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
// A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
// OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
// SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
// LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
// DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
// THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
// (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
// OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-->
