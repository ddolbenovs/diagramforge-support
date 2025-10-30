# Privacy Policy — DiagramForge

**Last updated:** 2025-10-31

This Privacy Policy describes how DiagramForge (the "App") handles information when used inside Confluence. DiagramForge is developed and maintained by an independent developer (ddolbenovs). The App's primary function is to render text-based diagrams by forwarding user-provided diagram source code to a Kroki-compatible rendering service and returning the resulting SVG to Confluence for display.

## Summary
- DiagramForge does **not** automatically collect analytics or personal data from Confluence users.
- Diagram source code provided by users is transmitted to the configured Kroki rendering endpoint (public `kroki.io` or a self-hosted Kroki instance) for on-demand rendering.
- Administrators may configure the Kroki endpoint in the App settings. For strict data control, we recommend using a self-hosted Kroki instance.

## Data processed and transmission
- **What is sent to Kroki:** the diagram type and the diagram source code (plain text). Diagram source may include any text the user enters, which could include personally identifiable information (PII) if the author inserts it.
- **Why it is sent:** to render the diagram into SVG and return the image to the Confluence page.
- **Where it is sent:** to the Kroki endpoint configured by the Confluence administrator or App user. This may be the public `https://kroki.io` service or a private instance.

## Storage and retention
- The App does not persist diagram source or rendered images beyond what is required for embedding in Confluence pages. Diagram source is forwarded to Kroki at render time and the returned SVG is embedded in the Confluence page.
- Support correspondence (issues, emails) may be stored by the developer for troubleshooting and is retained only as long as necessary to resolve the issue.

## Third parties
- Rendering is performed by Kroki or a compatible server. Use of the public `kroki.io` service is subject to Kroki's privacy practices. If you require strict data control, configure the App to use a private Kroki instance hosted within your infrastructure.
- If you submit support requests to the public repository or support channels, the contents of those reports (including sample diagram source and error messages) will be visible to support maintainers.

## Security
- DiagramForge does not access or transmit Confluence user credentials. Network traffic to the configured Kroki endpoint should use HTTPS; administrators should ensure TLS is enforced for private endpoints.
- For sensitive environments, host Kroki within your network and configure the App to use that private endpoint.

## Your choices and responsibilities
- **Administrators:** choose whether to use the public Kroki service or a self-hosted instance. Self-hosting is recommended for enterprise privacy requirements.
- **Users:** avoid including sensitive personal data in diagram source if you do not want that text transmitted to the configured Kroki endpoint.

## Contact
For support or privacy questions:
- Issues: https://github.com/ddolbenovs/diagramforge-support/issues

## Changes to this policy
This policy may be updated periodically. The "Last updated" date above reflects the latest revision.
