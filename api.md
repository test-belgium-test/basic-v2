---
layout: default
title: API Docs
permalink: /api/
---

<h1>API Documentation</h1>
<div id="swagger-ui"></div>

<!-- Swagger UI -->
<link rel="stylesheet" type="text/css" href="/docs/lib4ui/swagger-ui.css" />
<script src="/docs/lib4ui/swagger-ui-bundle.js" charset="UTF-8"></script>
<script src="/docs/lib4ui/swagger-ui-standalone-preset.js" charset="UTF-8"></script>

<script>
  window.onload = function () {
    SwaggerUIBundle({
      url: "/docs/technical_specs/basic.yaml",
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
