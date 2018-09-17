To run swagger UI:
    - Run npm install
    - Copy and paste aster-swagger.yaml file inside /node_modules/swagger-ui-dist
    - Change url parameter inside SwaggerUIBundle to "aster-swagger.yaml" as follows
        const ui = SwaggerUIBundle({
                url: "aster-swagger.yaml",
                dom_id: '#swagger-ui',
                deepLinking: true,
                presets: [
                  SwaggerUIBundle.presets.apis,
                  SwaggerUIStandalonePreset
                ],
                plugins: [
                  SwaggerUIBundle.plugins.DownloadUrl
                ],
                layout: "StandaloneLayout"
              })