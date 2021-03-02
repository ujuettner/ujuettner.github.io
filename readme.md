## Install Jekyll

```bash
ruby --version   # has to be >= 2.5.0
# install Gems into your home directory to avoid need for root permissions
export GEM_HOME="${HOME}/gems"
export PATH="${HOME}/gems/bin:${PATH}"
gem install jekyll bundler
bundle install
```

## Update Gems (e.g Jekyll)

```bash
bundle update
```

## Local Build of Site

```bash
bundle exec jekyll serve
```

Open http://127.0.0.1:4000/ in browser.

## Troubleshooting

Disable IPv6 (in case of persistent network problems):
```bash
sudo sysctl -w net.ipv6.conf.default.disable_ipv6=1
sudo sysctl -w net.ipv6.conf.all.disable_ipv6=1
```

## References

* [About GitHub Pages and Jekyll](https://help.github.com/en/github/working-with-github-pages/about-github-pages-and-jekyll)
* [Jekyll](https://jekyllrb.com/)
