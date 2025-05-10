---
layout: default
title: API Docs
permalink: /api/
---

<h1>API Documentation</h1>
<div id="swagger-ui"></div>

<link rel="stylesheet" type="text/css" href="/basic-v2/docs/lib4ui/swagger-ui.css" />
<script src="/basic-v2/docs/lib4ui/swagger-ui-bundle.js" charset="UTF-8"></script>
<script src="/basic-v2/docs/lib4ui/swagger-ui-standalone-preset.js" charset="UTF-8"></script>

<script>
  window.onload = function () {
    SwaggerUIBundle({
      url: "/basic-v2/docs/technical_specs/basic.yaml",
      dom_id: '#swagger-ui',
      deepLinking: true,
      presets: [
        SwaggerUIBundle.presets.apis,
        SwaggerUIStandalonePreset
      ],
      layout: "StandaloneLayout"
    });
  };
</script>
