# Humane Ecology Website

Scientific rigor, analytic acuity, infrastructure to make a difference.

## Custom Background Image

This site uses the Jekyll Modernist theme with a custom background image feature. You can specify any image from your `/images` directory as the background.

### How to Change the Background Image

1. Add your image to the `/images` directory
2. Edit `_config.yml` and update the `background_image` setting:

```yaml
background_image: /images/your-image.jpeg
```

3. To revert to the default theme background (dark slate grey), simply comment out or remove the `background_image` line in `_config.yml`

### Available Images

The following images are currently available in the `/images` directory:
- IMG_5710.jpeg (currently in use)
- 24A00137-B116-4D9A-A401-946BF7597AB3_1_105_c.jpeg
- 29D75C8C-B3E9-43F5-864B-2F8789B19923_1_105_c.jpeg
- 6E85793F-3A0A-47D1-95E9-81F2BD470887_1_105_c.jpeg
- C3853AC0-6305-4052-8EEC-12574F1B08FB_1_105_c.jpeg
- E07C52CA-6A92-4C55-9944-ABC9D14E12C9_1_105_c.jpeg
- FB189CCF-C9BB-4E07-A021-5FE33E409F3A_4_5005_c.jpeg

## Local Development

To run the site locally:

```bash
bundle install
bundle exec jekyll serve
```

Then visit `http://localhost:4000` in your browser.
