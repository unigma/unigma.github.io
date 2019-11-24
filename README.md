# UNIGMA Web

UNIST Enigma Games Website

## Usage

1. Clone this repository
2. Add a new post in `_posts/` directory with proper name format (as shown in previous posts)
3. Commit and PR

## Local Build

If you want to see the changes before pushing the blog to Github, do a local build.

1. [`gem install jekyll`](https://jekyllrb.com/docs/installation/#install-with-rubygems)
2. `gem install jekyll-seo-tag`
3. (`cd` to the blog directory, then:) `jekyll serve --watch --port 8000`
4. Go to `http://0.0.0.0:8000/` in your web browser.

*Note: In case you have set a `baseurl` different than `/` in `_config.yml`, go to `http://0.0.0.0:8000/BASEURL/` instead.*

### Local build using docker

```bash
docker run --rm -p 8000:8000 \
  --volume="LOCATION_OF_YOUR_JEKYLL_BLOG:/srv/jekyll" \
  -it tocttou/jekyll:3.5 \
  jekyll serve --watch --port 8000
```

Replace `LOCATION_OF_YOUR_JEKYLL_BLOG` with the full path of your blog repository. Visit `http://localhost:8000/` to access the blog.

*Note: In case you have set a `baseurl` different than `/` in `_config.yml`, go to `http://0.0.0.0:8000/BASEURL/` instead.*

### ToDo

*Note: All links in the site are prepended with `baseurl`. Default `baseurl` is `/`. Any other baseurl can be setup like `baseurl: /hacker-blog`, which makes the site available at `http://domain.name/hacker-blog`.*

Additionally, you may choose to set the following optional variables:

```yml
google_analytics: [Your Google Analytics tracking ID]
```

## License

CC0 1.0 Universal
