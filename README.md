# Pray n Push Hugo Theme

This is a customized, highly-optimized fork of the excellent Card-style Hugo theme (originally Stack). It has been exclusively tailored and enhanced for **Pray&Push**.

## 🌟 Custom Enhancements

This fork includes several exclusive feature upgrades and bug fixes that are not available in the original theme:

### 1. Click-to-Play YouTube Cover (Lite YouTube Embed)
We have completely overhauled the article header component to support high-performance YouTube video embeds. 
- **How it works:** Instead of loading a heavy YouTube iFrame immediately (which ruins page speed), the theme intercepts the featured image and overlays a centralized Play Button. The actual video player is only loaded and auto-played when the user actively clicks the cover.
- **Mobile Optimized:** Uses the rock-solid "Display Toggle" and `padding-bottom: 56.25%` responsive layout to ensure 100% compatibility and prevent layout collapsing on mobile devices (including old iOS Safari).
- **Usage:** Simply add the `youtube` parameter to your article's Front Matter:
  ```yaml
  title: "My Awesome Video Post"
  image: "featured.png"
  youtube: "DTrHAxusLJA" # Just the YouTube video ID
  ```

### 2. OpenGraph & Twitter Card Bug Fixes
- Fixed a critical case-sensitivity bug (`$image.permalink` to `$image.Permalink`) that previously prevented social media platforms (like Twitter, Facebook) and RSS feed readers from correctly parsing and displaying the article's featured image.

### 3. Modernized Hugo Syntax
- Eliminated all Hugo compilation warnings by upgrading deprecated syntaxes (e.g., changing `.Site.Data` to `site.Data` and removing unnecessary JSON outputs in `hugo.toml`).

## ⚙️ Setup & Usage
Since this is a private/customized fork, it is directly integrated via Git Submodules into the main Hugo blog repository.
Any future design updates, CSS tweaks, or component modifications should be committed directly to this repository (`hugo-theme-praynpush`).

## Copyright

Originally based on the GNU General Public License v3.0 theme designed by Jimmy Cai.
Customized and maintained by **Pray&Push**.
