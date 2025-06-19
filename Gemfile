# ────────────────────────────────────────────────────────────────
#  SOURCES RUBYGEMS
# ────────────────────────────────────────────────────────────────
source "https://rubygems.org"

# ────────────────────────────────────────────────────────────────
#  DÉPENDANCES JEKYLL / GITHUB PAGES
# ────────────────────────────────────────────────────────────────
# Le méta-gem « github-pages » embarque Jekyll 4.x + les bonnes versions
# de kramdown, rouge, etc. (celles autorisées par GitHub Pages).
gem "github-pages", group: :jekyll_plugins

# Thème Minimal-Mistakes (design moderne, responsive)
gem "minimal-mistakes-jekyll", group: :jekyll_plugins

# Cache d’inclusions utilisé par le thème
gem "jekyll-include-cache", group: :jekyll_plugins

# ────────────────────────────────────────────────────────────────
#  PLUGINS SUPPLÉMENTAIRES (déjà whitelistes par GitHub)
# ────────────────────────────────────────────────────────────────
gem "jekyll-feed", group: :jekyll_plugins   # flux RSS/Atom auto

# ────────────────────────────────────────────────────────────────
#  COMPATIBILITÉ WINDOWS & JRuby
# ────────────────────────────────────────────────────────────────
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
  gem "wdm", "~> 0.1"            # accélère le watcher sur Windows
end

# JRuby : verrouiller http_parser
gem "http_parser.rb", "~> 0.6.0", platforms: [:jruby]
