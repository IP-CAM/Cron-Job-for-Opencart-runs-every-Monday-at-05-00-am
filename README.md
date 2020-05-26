# Cron jobs

For **Opencart** installations many times we need to delete the contents of `/image/cache/` folder except **`index.html`**.  
`0   5   *   *   1   find /path-to-image-folder/image/cache/ -type f -not -name 'index.html' -delete >/dev/null 2>&1`
