# vim-quickrun-markdown-gfm

vim-quickrun-markdown-gfm converts a markdown buffer to html quickly by GitHub Markdown Rendering API.

## Install with Vundle

Add the following lines to your `.vimrc`:

```vim
Bundle 'thinca/vim-quickrun'
Bundle 'mattn/webapi-vim'
Bundle 'tyru/open-browser.vim'
Bundle 'superbrothers/vim-quickrun-markdown-gfm'
```

```vim
let g:quickrun_config = {
\   'markdown': {
\     'type': 'markdown/gfm',
\     'outputter': 'browser'
\   }
\ }
```

After execute `:BundleInstall`.

If you want to use this script on GitHub Enterprise:

```vim
let g:quickrun_markdown_gfm_github_api_url = 'https://<your-github-enterprise-hostname>/api/v3'
```

If you want to use a GitHub OAuth token:

```vim
let g:quickrun_markdown_gfm_github_token = '<your-github-oauth-token>'
```

## Usage

    :QuickRun markdown

For more information, see the help of vim-quickrun

    :help quickrun

## Requirements

- [curl and libcurl](http://curl.haxx.se/)
- [Markdown Rendering | GitHub API](http://developer.github.com/v3/markdown/)
- [thinca/vim-quickrun](https://github.com/thinca/vim-quickrun)
- [mattn/webapi-vim](https://github.com/mattn/webapi-vim)
- [tyru/open-browser.vim](https://github.com/tyru/open-browser.vim)
- [revolunet/sublimetext-markdown-preview](https://github.com/revolunet/sublimetext-markdown-preview)  
    `github.css`, `highlight.css`, `highlight.js`

## License

vim-quickrun-markdown-gfm is released under the [MIT License](http://www.opensource.org/licenses/MIT).

## Screenshots

![Screenshot 01](screenshots/ss01.png)
