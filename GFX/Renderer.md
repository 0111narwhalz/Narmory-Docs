# Renderer
The renderer visualizes a projectile in flight given a [[Render Data]].

## List of Renderers
- [[RendererNull]]: Invisible. Used to reduce graphical load when large quantities of projectiles are expected.
- [[RendererPellet]]: Renders a small pellet at the projectile's position.
- [[RendererTracer]]: Simple monochrome line traced between positions to model persistence of vision.