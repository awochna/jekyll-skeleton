# jekyll-skeleton #

[![Gem Version](https://badge.fury.io/rb/jekyll-skeleton.svg)](https://badge.fury.io/rb/jekyll-skeleton)

Super simple implementation of [Skeleton CSS](http://getskeleton.com) as a Jekyll theme.

## Why? ##

I got tired of heavy CSS frameworks (Bootstrap & Foundation) being large downloads and getting in my way of customizing my blog.
I know you can select only the components you want from each of these and throw away others, but that seemed like the opposite direction than I wanted to work from.

## Installation ##

Add this line to your Jekyll site's Gemfile:

```ruby
gem "jekyll-skeleton"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-skeleton
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-skeleton

This will give you some simple, basic layouts (nothing fancy) and the basic CSS.
It's just a skeleton, after all ;)

You can add custom CSS in `assets/style.css` in your Jekyll site and it'll automatically be included.

## Google Analytics ##

This theme has a google analytics helper for page views.
All you have to do is add something like the following to your `_config.yml`:

```
google_analytics: "UA-00000000-1"
anonymize_ip: true
```

Use whatever your UA code is.
The `anonymize_ip` option is to anonymize IP addresses when collecting tracking information.
Anonymizing IP information means you don't track any sort of personal data.

## Adding Related Posts ##

To list related posts at the end of a post, add the following line to your `_config.yaml`:

    include_related_posts: true

Then, the top 5 related posts will be listed.
See Jekyll's [docs](https://jekyllrb.com/docs/variables/#site-variables) for more information on what this means.

## Enabling comments via Disqus ##

If you have a Disqus account, you can enable comments for your posts in the same way as you do for Minima, by adding the following to your `_config.yml`:

```
disqus:
  shortname: my_disqus_shortname
```

Like in Minima, comments are enabled by default and appear only in a production environment (`JEKYLL_ENV=production`).

Adding `comments: false` to a post's YAML front matter turns off displaying comments for that post.

## Privacy Policy link ##

You can provide a link to your privacy policy in the footer of your site by specifying the URL in your `_config.yml` file.
Add the following:

```
privacy_policy_url: "/your-privacy-policy-url-here"
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/awochna/jekyll-skeleton. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Development

To set up your environment to develop this theme, run `bundle install`.

There is an example site in the `example/` folder using this theme that you can develop against.

## License

The theme is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

