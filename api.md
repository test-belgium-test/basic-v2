---
layout: default
title: API Docs
permalink: /api/
---

<h1>API Documentation</h1>
<div id="swagger-ui"></div>

<!-- Swagger UI -->
<link rel="stylesheet" href="https://unpkg.com/swagger-ui-dist/swagger-ui.css" />
<script src="https://unpkg.com/swagger-ui-dist/swagger-ui-bundle.js"></script>
<script src="https://unpkg.com/swagger-ui-dist/swagger-ui-standalone-preset.js"></script>

<script>
  window.onload = function () {
    SwaggerUIBundle({
      url: "/docs/technical_specs/basic.yaml",
      dom_id: "#swagger-ui",
      presets: [
        SwaggerUIBundle.presets.apis,
        SwaggerUIStandalonePreset
      ],
      layout: "StandaloneLayout"
    });
  };
</script>
