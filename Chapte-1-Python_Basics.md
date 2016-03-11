



<!DOCTYPE html>
<html lang="en" class=" is-copy-enabled is-u2f-enabled">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/frameworks-901bb74dd76b96d487bd6994b335b166cf71677c3a24de13ce68a5a7346806d2.css" integrity="sha256-kBu3TddrltSHvWmUszWxZs9xZ3w6JN4TzmilpzRoBtI=" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-164e36c95b8b2e7edffe11b313847cfb1784ec23bfc140b799037dee94f5a5fc.css" integrity="sha256-Fk42yVuLLn7f/hGzE4R8+xeE7CO/wUC3mQN97pT1pfw=" media="all" rel="stylesheet" />
    
    
    

    <link as="script" href="https://assets-cdn.github.com/assets/frameworks-e677f2022a5d36e8f5ad35d0fcb01f83f1cdb613eda0449f533197693bcc6bda.js" rel="preload" />
    <link as="script" href="https://assets-cdn.github.com/assets/github-2294152c3b0a63083bf2fb5d4cd4242f741f0240f42d9be0d37d0c26d448a0b4.js" rel="preload" />

    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=1020">
    
    
    <title>Automate-the-Boring-Stuff-with-Python-ChineseVersion/Chapte-1-Python_Basics.md at lingfeng-ch2 · lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" href="/apple-touch-icon.png">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="/apple-touch-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="/apple-touch-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="/apple-touch-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="/apple-touch-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon-180x180.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="https://avatars0.githubusercontent.com/u/5792174?v=3&amp;s=400" name="twitter:image:src" /><meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion" name="twitter:title" /><meta content="Automate-the-Boring-Stuff-with-Python-ChineseVersion - Automate the Boring Stuff with Python 中文翻译版，欢迎fork" name="twitter:description" />
      <meta content="https://avatars0.githubusercontent.com/u/5792174?v=3&amp;s=400" property="og:image" /><meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion" property="og:title" /><meta content="https://github.com/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion" property="og:url" /><meta content="Automate-the-Boring-Stuff-with-Python-ChineseVersion - Automate the Boring Stuff with Python 中文翻译版，欢迎fork" property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    <link rel="web-socket" href="wss://live.github.com/_sockets/NTc5MjE3NDo3MjBmNGE4NWZmMTUwMDU4YjI3YWVhNjgxYTRmZTRkYjpjODFmNjAzN2U1MmQ2OTkxZTZlM2EzYWQ3YjAyZWUwZjUxMDk2NjI1NGI1YmYwOTk1MmU1ZGVkMTNhMTgwNmYx--f98d3f5e52802c1ea67069d04fdedd4882a8a114">
    <meta name="pjax-timeout" content="1000">
    <link rel="sudo-modal" href="/sessions/sudo_modal">

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
<meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-analytics" content="UA-3769691-2">

<meta content="collector.githubapp.com" name="octolytics-host" /><meta content="github" name="octolytics-app-id" /><meta content="67C0B051:5B1E:50433DA:56E21824" name="octolytics-dimension-request_id" /><meta content="5792174" name="octolytics-actor-id" /><meta content="lisiyu" name="octolytics-actor-login" /><meta content="65fd026fb7c25ece5f1254a34d6c8fc502baaafc36fdc5596329a33187e8f0e9" name="octolytics-actor-hash" />
<meta content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" name="analytics-location" />



  <meta class="js-ga-set" name="dimension1" content="Logged In">



        <meta name="hostname" content="github.com">
    <meta name="user-login" content="lisiyu">

        <meta name="expected-hostname" content="github.com">
      <meta name="js-proxy-site-detection-payload" content="NzMzM2EwZDllZTZmNzEwYjNkMTZkN2ExODk5MjZjMjYwODZjN2I4N2RkY2JmYmFhZmY4NmY0ZGYzMDc2MjhjZXx7InJlbW90ZV9hZGRyZXNzIjoiMTAzLjE5Mi4xNzYuODEiLCJyZXF1ZXN0X2lkIjoiNjdDMEIwNTE6NUIxRTo1MDQzM0RBOjU2RTIxODI0In0=">

      <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#4078c0">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <meta content="587a43792f2b8ceeccf5f9dc0d3e4034ad13f12a" name="form-nonce" />

    <meta http-equiv="x-pjax-version" content="d43e17f845222c1cdf3bb926f9402651">
    

      
  <meta name="description" content="Automate-the-Boring-Stuff-with-Python-ChineseVersion - Automate the Boring Stuff with Python 中文翻译版，欢迎fork">
  <meta name="go-import" content="github.com/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion git https://github.com/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion.git">

  <meta content="5792174" name="octolytics-dimension-user_id" /><meta content="lisiyu" name="octolytics-dimension-user_login" /><meta content="52713790" name="octolytics-dimension-repository_id" /><meta content="lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="true" name="octolytics-dimension-repository_is_fork" /><meta content="34940813" name="octolytics-dimension-repository_parent_id" /><meta content="hanxiaomax/Automate-the-Boring-Stuff-with-Python-ChineseVersion" name="octolytics-dimension-repository_parent_nwo" /><meta content="34940813" name="octolytics-dimension-repository_network_root_id" /><meta content="hanxiaomax/Automate-the-Boring-Stuff-with-Python-ChineseVersion" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/commits/lingfeng-ch2.atom" rel="alternate" title="Recent Commits to Automate-the-Boring-Stuff-with-Python-ChineseVersion:lingfeng-ch2" type="application/atom+xml">


      <link rel="canonical" href="https://github.com/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/blob/lingfeng-ch2/Chapte-1-Python_Basics.md" data-pjax-transient>
  </head>


  <body class="logged_in   env-production windows vis-public fork page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>

    
    
    



      <div class="header header-logged-in true" role="banner">
  <div class="container clearfix">

    <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" data-ga-click="Header, go to dashboard, icon:logo">
  <svg aria-hidden="true" class="octicon octicon-mark-github" height="28" role="img" version="1.1" viewBox="0 0 16 16" width="28"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59 0.4 0.07 0.55-0.17 0.55-0.38 0-0.19-0.01-0.82-0.01-1.49-2.01 0.37-2.53-0.49-2.69-0.94-0.09-0.23-0.48-0.94-0.82-1.13-0.28-0.15-0.68-0.52-0.01-0.53 0.63-0.01 1.08 0.58 1.23 0.82 0.72 1.21 1.87 0.87 2.33 0.66 0.07-0.52 0.28-0.87 0.51-1.07-1.78-0.2-3.64-0.89-3.64-3.95 0-0.87 0.31-1.59 0.82-2.15-0.08-0.2-0.36-1.02 0.08-2.12 0 0 0.67-0.21 2.2 0.82 0.64-0.18 1.32-0.27 2-0.27 0.68 0 1.36 0.09 2 0.27 1.53-1.04 2.2-0.82 2.2-0.82 0.44 1.1 0.16 1.92 0.08 2.12 0.51 0.56 0.82 1.27 0.82 2.15 0 3.07-1.87 3.75-3.65 3.95 0.29 0.25 0.54 0.73 0.54 1.48 0 1.07-0.01 1.93-0.01 2.2 0 0.21 0.15 0.46 0.55 0.38C13.71 14.53 16 11.53 16 8 16 3.58 12.42 0 8 0z"></path></svg>
</a>


      <div class="site-search repo-scope js-site-search" role="search">
          <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <label class="js-chromeless-input-container form-control">
    <div class="scope-badge">This repository</div>
    <input type="text"
      class="js-site-search-focus js-site-search-field is-clearable chromeless-input"
      data-hotkey="s"
      name="q"
      placeholder="Search"
      aria-label="Search this repository"
      data-global-scope-placeholder="Search GitHub"
      data-repo-scope-placeholder="Search"
      tabindex="1"
      autocapitalize="off">
  </label>
</form>
      </div>

      <ul class="header-nav left" role="navigation">
        <li class="header-nav-item">
          <a href="/pulls" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:pulls context:user" data-hotkey="g p" data-selected-links="/pulls /pulls/assigned /pulls/mentioned /pulls">
            Pull requests
</a>        </li>
        <li class="header-nav-item">
          <a href="/issues" class="js-selected-navigation-item header-nav-link" data-ga-click="Header, click, Nav menu - item:issues context:user" data-hotkey="g i" data-selected-links="/issues /issues/assigned /issues/mentioned /issues">
            Issues
</a>        </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://gist.github.com/" data-ga-click="Header, go to gist, text:gist">Gist</a>
          </li>
      </ul>

    
<ul class="header-nav user-nav right" id="user-links">
  <li class="header-nav-item">
      <span class="js-socket-channel js-updatable-content"
        data-channel="notification-changed:lisiyu"
        data-url="/notifications/header">
      <a href="/notifications" aria-label="You have unread notifications" class="header-nav-link notification-indicator tooltipped tooltipped-s" data-ga-click="Header, go to notifications, icon:unread" data-hotkey="g n">
          <span class="mail-status unread"></span>
          <svg aria-hidden="true" class="octicon octicon-bell" height="16" role="img" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 12v1H0v-1l0.73-0.58c0.77-0.77 0.81-2.55 1.19-4.42 0.77-3.77 4.08-5 4.08-5 0-0.55 0.45-1 1-1s1 0.45 1 1c0 0 3.39 1.23 4.16 5 0.38 1.88 0.42 3.66 1.19 4.42l0.66 0.58z m-7 4c1.11 0 2-0.89 2-2H5c0 1.11 0.89 2 2 2z"></path></svg>
</a>  </span>

  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link tooltipped tooltipped-s js-menu-target" href="/new"
       aria-label="Create new…"
       data-ga-click="Header, create new, icon:add">
      <svg aria-hidden="true" class="octicon octicon-plus left" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 9H7v5H5V9H0V7h5V2h2v5h5v2z"></path></svg>
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <ul class="dropdown-menu dropdown-menu-sw">
        
<a class="dropdown-item" href="/new" data-ga-click="Header, create new repository">
  New repository
</a>


  <a class="dropdown-item" href="/organizations/new" data-ga-click="Header, create new organization">
    New organization
  </a>



  <div class="dropdown-divider"></div>
  <div class="dropdown-header">
    <span title="lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion">This repository</span>
  </div>
    <a class="dropdown-item" href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/settings/collaboration" data-ga-click="Header, create new collaborator">
      New collaborator
    </a>

      </ul>
    </div>
  </li>

  <li class="header-nav-item dropdown js-menu-container">
    <a class="header-nav-link name tooltipped tooltipped-sw js-menu-target" href="/lisiyu"
       aria-label="View profile and more"
       data-ga-click="Header, show menu, icon:avatar">
      <img alt="@lisiyu" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/5792174?v=3&amp;s=40" width="20" />
      <span class="dropdown-caret"></span>
    </a>

    <div class="dropdown-menu-content js-menu-content">
      <div class="dropdown-menu  dropdown-menu-sw">
        <div class=" dropdown-header header-nav-current-user css-truncate">
            Signed in as <strong class="css-truncate-target">lisiyu</strong>

        </div>


        <div class="dropdown-divider"></div>

          <a class="dropdown-item" href="/lisiyu" data-ga-click="Header, go to profile, text:your profile">
            Your profile
          </a>
        <a class="dropdown-item" href="/stars" data-ga-click="Header, go to starred repos, text:your stars">
          Your stars
        </a>
          <a class="dropdown-item" href="/explore" data-ga-click="Header, go to explore, text:explore">
            Explore
          </a>
          <a class="dropdown-item" href="/integrations" data-ga-click="Header, go to integrations, text:integrations">
            Integrations
          </a>
        <a class="dropdown-item" href="https://help.github.com" data-ga-click="Header, go to help, text:help">
          Help
        </a>


          <div class="dropdown-divider"></div>

          <a class="dropdown-item" href="/settings/profile" data-ga-click="Header, go to settings, icon:settings">
            Settings
          </a>

          <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/logout" class="logout-form" data-form-nonce="587a43792f2b8ceeccf5f9dc0d3e4034ad13f12a" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="SczUdYmyobhGjE4e8bnG47rGScVskiUc6LxCsbVSFMOYKtMz2w9RHVZ/VEvywzizz5gCa41BIEqaHXIJU8sNNA==" /></div>
            <button class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout">
              Sign out
            </button>
</form>
      </div>
    </div>
  </li>
</ul>


    
  </div>
</div>

      

      


    <div id="start-of-content" class="accessibility-aid"></div>

      <div id="js-flash-container">
</div>


    <div role="main" class="main-content">
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode">
    <div id="js-repo-pjax-container" class="context-loader-container js-repo-nav-next" data-pjax-container>
      
<div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav">
  <div class="container repohead-details-container">

    

<ul class="pagehead-actions">

  <li>
        <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/notifications/subscribe" class="js-social-container" data-autosubmit="true" data-form-nonce="587a43792f2b8ceeccf5f9dc0d3e4034ad13f12a" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="cMCsH1MrMzbbJ8+1UMv6sIR+piNIZ4p8B6Ka7NmI2+LLZB9pkPW4KmNukV6OZxesPzW6MYzXYCa0W6lBCMS95A==" /></div>      <input id="repository_id" name="repository_id" type="hidden" value="52713790" />

        <div class="select-menu js-menu-container js-select-menu">
          <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/subscription"
            class="btn btn-sm btn-with-count select-menu-button js-menu-target" role="button" tabindex="0" aria-haspopup="true"
            data-ga-click="Repository, click Watch settings, action:blob#show">
            <span class="js-select-button">
              <svg aria-hidden="true" class="octicon octicon-eye" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6c4.94 0 7.94-6 7.94-6S13 2 8.06 2z m-0.06 10c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4z m2-4c0 1.11-0.89 2-2 2s-2-0.89-2-2 0.89-2 2-2 2 0.89 2 2z"></path></svg>
              Unwatch
            </span>
          </a>
          <a class="social-count js-social-count" href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/watchers">
            1
          </a>

        <div class="select-menu-modal-holder">
          <div class="select-menu-modal subscription-menu-modal js-menu-content" aria-hidden="true">
            <div class="select-menu-header">
              <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75-1.48-1.48 3.75-3.75L0.77 4.25l1.48-1.48 3.75 3.75 3.75-3.75 1.48 1.48-3.75 3.75z"></path></svg>
              <span class="select-menu-title">Notifications</span>
            </div>

              <div class="select-menu-list js-navigation-container" role="menu">

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5L4 13 0 9l1.5-1.5 2.5 2.5 6.5-6.5 1.5 1.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input id="do_included" name="do" type="radio" value="included" />
                    <span class="select-menu-item-heading">Not watching</span>
                    <span class="description">Be notified when participating or @mentioned.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-eye" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6c4.94 0 7.94-6 7.94-6S13 2 8.06 2z m-0.06 10c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4z m2-4c0 1.11-0.89 2-2 2s-2-0.89-2-2 0.89-2 2-2 2 0.89 2 2z"></path></svg>
                      Watch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5L4 13 0 9l1.5-1.5 2.5 2.5 6.5-6.5 1.5 1.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input checked="checked" id="do_subscribed" name="do" type="radio" value="subscribed" />
                    <span class="select-menu-item-heading">Watching</span>
                    <span class="description">Be notified of all conversations.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-eye" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6c4.94 0 7.94-6 7.94-6S13 2 8.06 2z m-0.06 10c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4z m2-4c0 1.11-0.89 2-2 2s-2-0.89-2-2 0.89-2 2-2 2 0.89 2 2z"></path></svg>
                      Unwatch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5L4 13 0 9l1.5-1.5 2.5 2.5 6.5-6.5 1.5 1.5z"></path></svg>
                  <div class="select-menu-item-text">
                    <input id="do_ignore" name="do" type="radio" value="ignore" />
                    <span class="select-menu-item-heading">Ignoring</span>
                    <span class="description">Never be notified.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg aria-hidden="true" class="octicon octicon-mute" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M8 2.81v10.38c0 0.67-0.81 1-1.28 0.53L3 10H1c-0.55 0-1-0.45-1-1V7c0-0.55 0.45-1 1-1h2l3.72-3.72c0.47-0.47 1.28-0.14 1.28 0.53z m7.53 3.22l-1.06-1.06-1.97 1.97-1.97-1.97-1.06 1.06 1.97 1.97-1.97 1.97 1.06 1.06 1.97-1.97 1.97 1.97 1.06-1.06-1.97-1.97 1.97-1.97z"></path></svg>
                      Stop ignoring
                    </span>
                  </div>
                </div>

              </div>

            </div>
          </div>
        </div>
</form>
  </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">

    <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/unstar" class="js-toggler-form starred" data-form-nonce="587a43792f2b8ceeccf5f9dc0d3e4034ad13f12a" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="sV+z+xCcZT6N12XMeV4cdtK/XSzHQXBvdUWOr8hSYxlaZGY4RKicN+EEftIvSgr5hDoinqHpLiHoRWS1WE3Qcw==" /></div>
      <button
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <svg aria-hidden="true" class="octicon octicon-star" height="16" role="img" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 6l-4.9-0.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14l4.33-2.33 4.33 2.33L10.4 9.26 14 6z"></path></svg>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/stargazers">
          0
        </a>
</form>
    <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/star" class="js-toggler-form unstarred" data-form-nonce="587a43792f2b8ceeccf5f9dc0d3e4034ad13f12a" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="GZcNO309KzqIHJuqpNilHuj4VsvnRVcW1i3fubDzg2nYiClz+ktnci0o4wFa7ZAxpZKEpSKg13CfQpRDLvDydA==" /></div>
      <button
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Star this repository" title="Star lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <svg aria-hidden="true" class="octicon octicon-star" height="16" role="img" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 6l-4.9-0.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14l4.33-2.33 4.33 2.33L10.4 9.26 14 6z"></path></svg>
        Star
      </button>
        <a class="social-count js-social-count" href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/stargazers">
          0
        </a>
</form>  </div>

  </li>

  <li>
          <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/fork" class="btn-with-count" data-form-nonce="587a43792f2b8ceeccf5f9dc0d3e4034ad13f12a" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="9NdhE7CNX+V6Z+Z1pRcadimj7HJzu2ZqR0CnVAIkqzJa/VY4ZDbroXCtrSnD5vnaC7MdvPfJx0VK3pxRDoGfAQ==" /></div>
            <button
                type="submit"
                class="btn btn-sm btn-with-count"
                data-ga-click="Repository, show fork modal, action:blob#show; text:Fork"
                title="Fork your own copy of lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion to your account"
                aria-label="Fork your own copy of lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion to your account">
              <svg aria-hidden="true" class="octicon octicon-repo-forked" height="16" role="img" version="1.1" viewBox="0 0 10 16" width="10"><path d="M8 1c-1.11 0-2 0.89-2 2 0 0.73 0.41 1.38 1 1.72v1.28L5 8 3 6v-1.28c0.59-0.34 1-0.98 1-1.72 0-1.11-0.89-2-2-2S0 1.89 0 3c0 0.73 0.41 1.38 1 1.72v1.78l3 3v1.78c-0.59 0.34-1 0.98-1 1.72 0 1.11 0.89 2 2 2s2-0.89 2-2c0-0.73-0.41-1.38-1-1.72V9.5l3-3V4.72c0.59-0.34 1-0.98 1-1.72 0-1.11-0.89-2-2-2zM2 4.2c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z m3 10c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z m3-10c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z"></path></svg>
              Fork
            </button>
</form>
    <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/network" class="social-count">
      3
    </a>
  </li>
</ul>

    <h1 class="entry-title public ">
  <svg aria-hidden="true" class="octicon octicon-repo-forked" height="16" role="img" version="1.1" viewBox="0 0 10 16" width="10"><path d="M8 1c-1.11 0-2 0.89-2 2 0 0.73 0.41 1.38 1 1.72v1.28L5 8 3 6v-1.28c0.59-0.34 1-0.98 1-1.72 0-1.11-0.89-2-2-2S0 1.89 0 3c0 0.73 0.41 1.38 1 1.72v1.78l3 3v1.78c-0.59 0.34-1 0.98-1 1.72 0 1.11 0.89 2 2 2s2-0.89 2-2c0-0.73-0.41-1.38-1-1.72V9.5l3-3V4.72c0.59-0.34 1-0.98 1-1.72 0-1.11-0.89-2-2-2zM2 4.2c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z m3 10c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z m3-10c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z"></path></svg>
  <span class="author" itemprop="author"><a href="/lisiyu" class="url fn" rel="author">lisiyu</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion" data-pjax="#js-repo-pjax-container">Automate-the-Boring-Stuff-with-Python-ChineseVersion</a></strong>

  <span class="page-context-loader">
    <img alt="" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
  </span>

    <span class="fork-flag">
      <span class="text">forked from <a href="/hanxiaomax/Automate-the-Boring-Stuff-with-Python-ChineseVersion">hanxiaomax/Automate-the-Boring-Stuff-with-Python-ChineseVersion</a></span>
    </span>
</h1>

  </div>
  <div class="container">
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax js-octicon-loaders"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
     role="navigation"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/tree/lingfeng-ch2" aria-selected="true" class="js-selected-navigation-item selected reponav-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/tree/lingfeng-ch2" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-code" height="16" role="img" version="1.1" viewBox="0 0 14 16" width="14"><path d="M9.5 3l-1.5 1.5 3.5 3.5L8 11.5l1.5 1.5 4.5-5L9.5 3zM4.5 3L0 8l4.5 5 1.5-1.5L2.5 8l3.5-3.5L4.5 3z"></path></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>


  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/pulls" class="js-selected-navigation-item reponav-item" data-hotkey="g p" data-selected-links="repo_pulls /lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/pulls" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-git-pull-request" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M11 11.28c0-1.73 0-6.28 0-6.28-0.03-0.78-0.34-1.47-0.94-2.06s-1.28-0.91-2.06-0.94c0 0-1.02 0-1 0V0L4 3l3 3V4h1c0.27 0.02 0.48 0.11 0.69 0.31s0.3 0.42 0.31 0.69v6.28c-0.59 0.34-1 0.98-1 1.72 0 1.11 0.89 2 2 2s2-0.89 2-2c0-0.73-0.41-1.38-1-1.72z m-1 2.92c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2zM4 3c0-1.11-0.89-2-2-2S0 1.89 0 3c0 0.73 0.41 1.38 1 1.72 0 1.55 0 5.56 0 6.56-0.59 0.34-1 0.98-1 1.72 0 1.11 0.89 2 2 2s2-0.89 2-2c0-0.73-0.41-1.38-1-1.72V4.72c0.59-0.34 1-0.98 1-1.72z m-0.8 10c0 0.66-0.55 1.2-1.2 1.2s-1.2-0.55-1.2-1.2 0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2z m-1.2-8.8c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z"></path></svg>
      <span itemprop="name">Pull requests</span>
      <span class="counter">0</span>
      <meta itemprop="position" content="3">
</a>  </span>

    <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/wiki" class="js-selected-navigation-item reponav-item" data-hotkey="g w" data-selected-links="repo_wiki /lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/wiki">
      <svg aria-hidden="true" class="octicon octicon-book" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M2 5h4v1H2v-1z m0 3h4v-1H2v1z m0 2h4v-1H2v1z m11-5H9v1h4v-1z m0 2H9v1h4v-1z m0 2H9v1h4v-1z m2-6v9c0 0.55-0.45 1-1 1H8.5l-1 1-1-1H1c-0.55 0-1-0.45-1-1V3c0-0.55 0.45-1 1-1h5.5l1 1 1-1h5.5c0.55 0 1 0.45 1 1z m-8 0.5l-0.5-0.5H1v9h6V3.5z m7-0.5H8.5l-0.5 0.5v8.5h6V3z"></path></svg>
      Wiki
</a>
  <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/pulse" class="js-selected-navigation-item reponav-item" data-selected-links="pulse /lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/pulse">
    <svg aria-hidden="true" class="octicon octicon-pulse" height="16" role="img" version="1.1" viewBox="0 0 14 16" width="14"><path d="M11.5 8L8.8 5.4 6.6 8.5 5.5 1.6 2.38 8H0V10h3.6L4.5 8.2l0.9 5.4L9 8.5l1.6 1.5H14V8H11.5z"></path></svg>
    Pulse
</a>
  <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/graphs" class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors /lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/graphs">
    <svg aria-hidden="true" class="octicon octicon-graph" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M16 14v1H0V0h1v14h15z m-11-1H3V8h2v5z m4 0H7V3h2v10z m4 0H11V6h2v7z"></path></svg>
    Graphs
</a>
    <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/settings" class="js-selected-navigation-item reponav-item" data-selected-links="repo_settings repo_branch_settings hooks /lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/settings">
      <svg aria-hidden="true" class="octicon octicon-gear" height="16" role="img" version="1.1" viewBox="0 0 14 16" width="14"><path d="M14 8.77V7.17l-1.94-0.64-0.45-1.09 0.88-1.84-1.13-1.13-1.81 0.91-1.09-0.45-0.69-1.92H6.17l-0.63 1.94-1.11 0.45-1.84-0.88-1.13 1.13 0.91 1.81-0.45 1.09L0 7.23v1.59l1.94 0.64 0.45 1.09-0.88 1.84 1.13 1.13 1.81-0.91 1.09 0.45 0.69 1.92h1.59l0.63-1.94 1.11-0.45 1.84 0.88 1.13-1.13-0.92-1.81 0.47-1.09 1.92-0.69zM7 11c-1.66 0-3-1.34-3-3s1.34-3 3-3 3 1.34 3 3-1.34 3-3 3z"></path></svg>
      Settings
</a>
</nav>

  </div>
</div>

<div class="container new-discussion-timeline experiment-repo-nav">
  <div class="repository-content">

    

<a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/blob/7dadd67eb3e2cf7e88646135a5ca70737f7a5638/Chapte-1-Python_Basics.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:592815c9feb3d18b4781f86cd193e92b -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu js-menu-container js-select-menu left">
  <button class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    title="lingfeng-ch2"
    type="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">lingfeng-ch2</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75-1.48-1.48 3.75-3.75L0.77 4.25l1.48-1.48 3.75 3.75 3.75-3.75 1.48 1.48-3.75 3.75z"></path></svg>
        <span class="select-menu-title">Switch branches/tags</span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Find or create a branch…" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Find or create a branch…">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Find or create a branch…" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/blob/lingfeng-ch2/Chapte-1-Python_Basics.md"
               data-name="lingfeng-ch2"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5L4 13 0 9l1.5-1.5 2.5 2.5 6.5-6.5 1.5 1.5z"></path></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text" title="lingfeng-ch2">
                lingfeng-ch2
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
               href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/blob/lisiyu/Chapte-1-Python_Basics.md"
               data-name="lisiyu"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5L4 13 0 9l1.5-1.5 2.5 2.5 6.5-6.5 1.5 1.5z"></path></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text" title="lisiyu">
                lisiyu
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
               href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/blob/master/Chapte-1-Python_Basics.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M12 5L4 13 0 9l1.5-1.5 2.5 2.5 6.5-6.5 1.5 1.5z"></path></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text" title="master">
                master
              </span>
            </a>
        </div>

          <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/branches" class="js-create-branch select-menu-item select-menu-new-item-form js-navigation-item js-new-item-form" data-form-nonce="587a43792f2b8ceeccf5f9dc0d3e4034ad13f12a" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="zT3wWSxTfyQTWIlDLdI/JjjQb3e59MEcA9mAGJyz8XZ5+/FhLFiuNw7elpqwNrYzEYk0f6qsqb9oS9I9liHpeA==" /></div>
          <svg aria-hidden="true" class="octicon octicon-git-branch select-menu-item-icon" height="16" role="img" version="1.1" viewBox="0 0 10 16" width="10"><path d="M10 5c0-1.11-0.89-2-2-2s-2 0.89-2 2c0 0.73 0.41 1.38 1 1.72v0.3c-0.02 0.52-0.23 0.98-0.63 1.38s-0.86 0.61-1.38 0.63c-0.83 0.02-1.48 0.16-2 0.45V4.72c0.59-0.34 1-0.98 1-1.72 0-1.11-0.89-2-2-2S0 1.89 0 3c0 0.73 0.41 1.38 1 1.72v6.56C0.41 11.63 0 12.27 0 13c0 1.11 0.89 2 2 2s2-0.89 2-2c0-0.53-0.2-1-0.53-1.36 0.09-0.06 0.48-0.41 0.59-0.47 0.25-0.11 0.56-0.17 0.94-0.17 1.05-0.05 1.95-0.45 2.75-1.25s1.2-1.98 1.25-3.02h-0.02c0.61-0.36 1.02-1 1.02-1.73zM2 1.8c0.66 0 1.2 0.55 1.2 1.2s-0.55 1.2-1.2 1.2-1.2-0.55-1.2-1.2 0.55-1.2 1.2-1.2z m0 12.41c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z m6-8c-0.66 0-1.2-0.55-1.2-1.2s0.55-1.2 1.2-1.2 1.2 0.55 1.2 1.2-0.55 1.2-1.2 1.2z"></path></svg>
            <div class="select-menu-item-text">
              <span class="select-menu-item-heading">Create branch: <span class="js-new-item-name"></span></span>
              <span class="description">from ‘lingfeng-ch2’</span>
            </div>
            <input type="hidden" name="name" id="name" class="js-new-item-value">
            <input type="hidden" name="branch" id="branch" value="lingfeng-ch2">
            <input type="hidden" name="path" id="path" value="Chapte-1-Python_Basics.md">
</form>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

  <div class="btn-group right">
    <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/find/lingfeng-ch2"
          class="js-show-file-finder btn btn-sm"
          data-pjax
          data-hotkey="t">
      Find file
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button">Copy path</button>
  </div>
  <div class="breadcrumb js-zeroclipboard-target">
    <span class="repo-root js-repo-root"><span class="js-path-segment"><a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/tree/lingfeng-ch2"><span>Automate-the-Boring-Stuff-with-Python-ChineseVersion</span></a></span></span><span class="separator">/</span><strong class="final-path">Chapte-1-Python_Basics.md</strong>
  </div>
</div>

<include-fragment class="commit-tease" src="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/contributors/lingfeng-ch2/Chapte-1-Python_Basics.md">
  <div>
    Fetching contributors&hellip;
  </div>

  <div class="commit-tease-contributors">
    <img alt="" class="loader-loading left" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32-EAF2F5.gif" width="16" />
    <span class="loader-error">Cannot retrieve contributors at this time</span>
  </div>
</include-fragment>
<div class="file">
  <div class="file-header">
  <div class="file-actions">

    <div class="btn-group">
      <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/raw/lingfeng-ch2/Chapte-1-Python_Basics.md" class="btn btn-sm " id="raw-url">Raw</a>
        <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/blame/lingfeng-ch2/Chapte-1-Python_Basics.md" class="btn btn-sm js-update-url-with-hash">Blame</a>
      <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/commits/lingfeng-ch2/Chapte-1-Python_Basics.md" class="btn btn-sm " rel="nofollow">History</a>
    </div>

        <a class="btn-octicon tooltipped tooltipped-nw"
           href="github-windows://openRepo/https://github.com/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion?branch=lingfeng-ch2&amp;filepath=Chapte-1-Python_Basics.md"
           aria-label="Open this file in GitHub Desktop"
           data-ga-click="Repository, open with desktop, type:windows">
            <svg aria-hidden="true" class="octicon octicon-device-desktop" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M15 2H1c-0.55 0-1 0.45-1 1v9c0 0.55 0.45 1 1 1h5.34c-0.25 0.61-0.86 1.39-2.34 2h8c-1.48-0.61-2.09-1.39-2.34-2h5.34c0.55 0 1-0.45 1-1V3c0-0.55-0.45-1-1-1z m0 9H1V3h14v8z"></path></svg>
        </a>

        <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/edit/lingfeng-ch2/Chapte-1-Python_Basics.md" class="inline-form js-update-url-with-hash" data-form-nonce="587a43792f2b8ceeccf5f9dc0d3e4034ad13f12a" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="kJI1uLjq0r8cdkdl5D8IgeZbslfx2vKN+PUmHjQqGmIn6UVJAiI7rxy7cs8cv3cDIYYGJWhXb3PwU+5sYTWfVQ==" /></div>
          <button class="btn-octicon tooltipped tooltipped-nw" type="submit"
            aria-label="Edit this file" data-hotkey="e" data-disable-with>
            <svg aria-hidden="true" class="octicon octicon-pencil" height="16" role="img" version="1.1" viewBox="0 0 14 16" width="14"><path d="M0 12v3h3l8-8-3-3L0 12z m3 2H1V12h1v1h1v1z m10.3-9.3l-1.3 1.3-3-3 1.3-1.3c0.39-0.39 1.02-0.39 1.41 0l1.59 1.59c0.39 0.39 0.39 1.02 0 1.41z"></path></svg>
          </button>
</form>        <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/delete/lingfeng-ch2/Chapte-1-Python_Basics.md" class="inline-form" data-form-nonce="587a43792f2b8ceeccf5f9dc0d3e4034ad13f12a" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="wIGjnIOOTvX674gHw348IvbIbd9Rw2L/ymIOj6wU73ll7uhMsYexiMsKlU4DwY3T9yj2pLZbSoEvsmFov58rsA==" /></div>
          <button class="btn-octicon btn-octicon-danger tooltipped tooltipped-nw" type="submit"
            aria-label="Delete this file" data-disable-with>
            <svg aria-hidden="true" class="octicon octicon-trashcan" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M10 2H8c0-0.55-0.45-1-1-1H4c-0.55 0-1 0.45-1 1H1c-0.55 0-1 0.45-1 1v1c0 0.55 0.45 1 1 1v9c0 0.55 0.45 1 1 1h7c0.55 0 1-0.45 1-1V5c0.55 0 1-0.45 1-1v-1c0-0.55-0.45-1-1-1z m-1 12H2V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9z m1-10H1v-1h9v1z"></path></svg>
          </button>
</form>  </div>

  <div class="file-info">
      758 lines (541 sloc)
      <span class="file-info-divider"></span>
    46 KB
  </div>
</div>

  
  <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-chapter-1--python-basics" class="anchor" href="#chapter-1--python-basics" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Chapter 1 – Python Basics</h1>

<h1><a id="user-content-第一章-python基础" class="anchor" href="#第一章-python基础" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>第一章—— Python基础</h1>

<h2><a id="user-content-python-basics" class="anchor" href="#python-basics" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Python Basics</h2>

<h2><a id="user-content-python基础" class="anchor" href="#python基础" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Python基础</h2>

<p>The Python programming language has a wide range of syntactical constructions, standard library functions, and interactive development environment features. Fortunately, you can ignore most of that; you just need to learn enough to write some handy little programs.
You will, however, have to learn some basic programming concepts before you can do anything. Like a wizard-in-training, you might think these concepts seem arcane and tedious, but with some knowledge and practice, you’ll be able to command your computer like a magic wand to perform incredible feats.</p>

<p>Python这门编程语言有很多句法结构，标准库函数，和交互式开发环境特性。幸运的事，其中大部分你都可以忽略；你只需要学习一些知识，让你能够随手编写小程序即可。然而，你需要在开始前学习一些编程的基本概念。像见习巫师一样，你可能会认为这些概念看上去晦涩又乏味，但是具备了一定的知识，加上一些练习，你就可以像使用魔杖那样，让你的电脑完成了不起的工作</p>

<p>This chapter has a few examples that encourage you to type into the interactive shell, which lets you execute Python instructions one at a time and shows you the results instantly. Using the interactive shell is great for learning what basic Python instructions do, so give it a try as you follow along. You’ll remember the things you do much better than the things you only read.</p>

<p>本章有几个例子，鼓励你在交互式shell中输入它们，你可以在此一次执行一条Python指令，并马上将结果显示给你。使用交互式shell对于学习Python基本指令非常有帮助，所以请在接下来尝试一下。与那些你读到的东西相比，那些你做了的事情你会记得更牢。</p>

<h2><a id="user-content-entering-expressions-into-the-interactive-shell" class="anchor" href="#entering-expressions-into-the-interactive-shell" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Entering Expressions into the Interactive Shell</h2>

<h2><a id="user-content-在交互式shell中输入表达式" class="anchor" href="#在交互式shell中输入表达式" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>在交互式shell中输入表达式</h2>

<p>You run the interactive shell by launching IDLE, which you installed with Python in the introduction. On Windows, open the Start menu, select All Programs ▸ Python 3.3, and then select IDLE (Python GUI). On OS X, select Applications ▸ MacPython 3.3 ▸ IDLE. On Ubuntu, open a new Terminal window and enter idle3.
A window with the &gt;&gt;&gt; prompt should appear; that’s the interactive shell. Enter 2 + 2 at the prompt to have Python do some simple math.</p>

<p>你可以通过启动IDLE来运行交互式shell，IDLE在引言一章已经随Python一起安装了。在Windos上，点击开始菜单，选择全部程序 ▸Python 3.3，然后选择IDLE (Python GUI)。在OS X系统上，选择应用程序MacPython 3.3 ▸ IDLE。在Ubuntu上，打开终端窗口，输入<strong>idle3</strong>。</p>

<p>A window with the &gt;&gt;&gt; prompt should appear; that’s the interactive shell. Enter 2 + 2 at the prompt to have Python do some simple math.</p>

<p>一个带有&gt;&gt;&gt;提示符的窗口应该会出现；这就是交互式shell。
输入2 + 2可以让Python进行一次简单的数学计算。</p>

<pre><code>&gt;&gt;&gt; 2 + 2
4
</code></pre>

<p>The IDLE window should now show some text like this:
IDLE窗口现在应该显示如下的文本：</p>

<pre><code>Python 3.3.2 (v3.3.2:d047928ae3f6, May 16 2013, 00:06:53) [MSC v.1600 64 bit
(AMD64)] on win32
Type "copyright", "credits" or "license()" for more information.
&gt;&gt;&gt; 2 + 2
4
&gt;&gt;&gt;
</code></pre>

<p>In Python, 2 + 2 is called an expression, which is the most basic kind of programming instruction in the language. Expressions consist of values (such as 2) and operators (such as +), and they can always evaluate (that is, reduce) down to a single value. That means you can use expressions anywhere in Python code that you could also use a value.
In the previous example, 2 + 2 is evaluated down to a single value, 4. A single value with no operators is also considered an expression, though it evaluates only to itself, as shown here:</p>

<p>在Python中，2 + 2称之为表达式，是这个语言中最基本的一种程序指令。表达式包括值（比如2）以及操作符（比如＋），它总是会进行求值（减少变量），变为一个值。这就意味着在Python中，任何你可以使用表达式的地方你都可以使用一个值。在前面的例子中，2 + 2会求值得到一个单一的值4。一个不带有操作符的单一的值也被看做是表达式，尽管它只会求其本身的值，就像下面这样：</p>

<pre><code>&gt;&gt;&gt; 2
2
</code></pre>

<h3><a id="user-content-errors-are-okay" class="anchor" href="#errors-are-okay" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>ERRORS ARE OKAY!</h3>

<h3><a id="user-content-有错误没关系" class="anchor" href="#有错误没关系" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>有错误，没关系！</h3>

<p>Programs will crash if they contain code the computer can’t understand, which will cause Python to show an error message. An error message won’t break your computer, though, so don’t be afraid to make mistakes. A crash just means the program stopped running unexpectedly.
If you want to know more about an error message, you can search for the exact message text online to find out more about that specific error. You can also check out the resources at <a href="http://nostarch.com/automatestuff/">http://nostarch.com/automatestuff/</a> to see a list of common Python error messages and their meanings.</p>

<p>如果包含了电脑无法理解的指令，程序就会崩溃，也就会让Python显示错误信息。一条错误信息并不会弄坏你的电脑。所以并不要害怕犯错误。崩溃意味着程序突然停止工作。如果你想要了解更多关于错误信息的知识，你可以在网上搜索这条信息来找到更多关于这条特定信息的内容。你也可以查看这个网站的资源<a href="http://nostarch.com/automatestuff/">http://nostarch.com/automatestuff/</a>来看一下常见的Python错误信息以及它们代表的意思。</p>

<p>There are plenty of other operators you can use in Python expressions, too. For example, Table 1-1 lists all the math operators in Python.</p>

<p>还有很多你可以在Python表达式中使用的操作符。例如，表1-1列出了Python中所有的数学操作符</p>

<table><thead>
<tr>
<th align="center">Operator</th>
<th align="center">Operation</th>
<th align="center">Example</th>
<th align="center">Evaluates to...</th>
</tr>
</thead><tbody>
<tr>
<td align="center"><code>**</code></td>
<td align="center">Exponent</td>
<td align="center">2 ** 3</td>
<td align="center">8</td>
</tr>
<tr>
<td align="center"><code>%</code></td>
<td align="center">Modulus/remainder</td>
<td align="center">22 % 8</td>
<td align="center">6</td>
</tr>
<tr>
<td align="center"><code>//</code></td>
<td align="center">Integer division/floored quotient</td>
<td align="center">28//8</td>
<td align="center">2</td>
</tr>
<tr>
<td align="center"><code>/</code></td>
<td align="center">Division</td>
<td align="center">22 / 8</td>
<td align="center">2.75</td>
</tr>
<tr>
<td align="center"><code>*</code></td>
<td align="center">Multiplication</td>
<td align="center">3 * 5</td>
<td align="center">15</td>
</tr>
<tr>
<td align="center"><code>-</code></td>
<td align="center">Subtraction</td>
<td align="center">5-2</td>
<td align="center">3</td>
</tr>
<tr>
<td align="center"><code>+</code></td>
<td align="center">Addition</td>
<td align="center">2+2</td>
<td align="center">4</td>
</tr>
</tbody></table>

<table><thead>
<tr>
<th align="center">操作符</th>
<th align="center">操作</th>
<th align="center">实例</th>
<th align="center">求值</th>
</tr>
</thead><tbody>
<tr>
<td align="center"><code>**</code></td>
<td align="center">指数</td>
<td align="center">2 ** 3</td>
<td align="center">8</td>
</tr>
<tr>
<td align="center"><code>%</code></td>
<td align="center">取模/求余</td>
<td align="center">22 % 8</td>
<td align="center">6</td>
</tr>
<tr>
<td align="center"><code>//</code></td>
<td align="center">整除/商向下取整</td>
<td align="center">28//8</td>
<td align="center">2</td>
</tr>
<tr>
<td align="center"><code>/</code></td>
<td align="center">除法</td>
<td align="center">22 / 8</td>
<td align="center">2.75</td>
</tr>
<tr>
<td align="center"><code>*</code></td>
<td align="center">乘法</td>
<td align="center">3 * 5</td>
<td align="center">15</td>
</tr>
<tr>
<td align="center"><code>-</code></td>
<td align="center">减法</td>
<td align="center">5-2</td>
<td align="center">3</td>
</tr>
<tr>
<td align="center"><code>+</code></td>
<td align="center">加法</td>
<td align="center">2+2</td>
<td align="center">4</td>
</tr>
</tbody></table>

<p>The order of operations (also called precedence) of Python math operators is similar to that of mathematics. The ** operator is evaluated first; the *, /, //, and % operators are evaluated next, from left to right; and the + and - operators are evaluated last (also from left to right). You can use parentheses to override the usual precedence if you need to. Enter the following expressions into the interactive shell:</p>

<p>Python算术运算符的顺序（也叫做优先级）和数学里面是一样的。<code>**</code>首先被计算；<code>*</code>, <code>/</code>, <code>//</code>, 和 <code>%</code>次之，从左向右依次进行；<code>+</code>和<code>-</code>最后进行（同样也是从左到右）。如果需要的话你可以使用括号来手动控制优先级。在交互式shell中输入下面的表达式：</p>

<pre><code>&gt;&gt;&gt; 2 + 3 * 6
20
&gt;&gt;&gt; (2 + 3) * 6
30
&gt;&gt;&gt; 48565878 * 578453
28093077826734
&gt;&gt;&gt; 2 ** 8
256
&gt;&gt;&gt; 23 / 7
3.2857142857142856
&gt;&gt;&gt; 23 // 7
3
&gt;&gt;&gt; 23 % 7
2
&gt;&gt;&gt; 2     +            2
4
&gt;&gt;&gt; (5 - 1) * ((7 + 1) / (3 - 1))
16.0
</code></pre>

<p>In each case, you as the programmer must enter the expression, but Python does the hard part of evaluating it down to a single value. Python will keep evaluating parts of the expression until it becomes a single value, as shown in Figure 1-1.</p>

<p>在每一个例子中，你作为程序员，需要输入指令，然而Python做了最复杂的工作，把表达式求解为一个值。Python会不断求解表达式的各个部分知道它变为一个值，如图1-1所示。</p>

<p>These rules for putting operators and values together to form expressions are a fundamental part of Python as a programming language, just like the grammar rules that help us communicate. Here’s an example:</p>

<p>这些把操作符和变量放在一起构成表达式的规则，是Python这门编程语言的基础，就像帮助我们交流的语法一样。这里有一个例子：</p>

<ul>
<li>This is a grammatically correct English sentence.</li>
<li><p>This grammatically is sentence not English correct a.  </p></li>
<li><p>这是一个语法正确的中文句子  </p></li>
<li>这是语法是句子不是中文正确的一个</li>
</ul>

<p>The second line is difficult to parse because it doesn’t follow the rules of English. Similarly, if you type in a bad Python instruction, Python won’t be able to understand it and will display a SyntaxError error message, as shown here:</p>

<p>第二行难以解析因为它没有遵循中文的语法。同样的，如果你输入了一个错误的Python指令，Python不能够理解它并且会输出一个SyntaxError（语法错误）的错误信息，如下所示：</p>

<pre><code>&gt;&gt;&gt; 5 +
  File "&lt;stdin&gt;", line 1
    5 +
      ^
SyntaxError: invalid syntax
&gt;&gt;&gt; 42 + 5 + * 2
  File "&lt;stdin&gt;", line 1
    42 + 5 + * 2
             ^
SyntaxError: invalid syntax
</code></pre>

<p>You can always test to see whether an instruction works by typing it into the interactive shell. Don’t worry about breaking the computer: The worst thing that could happen is that Python responds with an error message. Professional software developers get error messages while writing code all the time.
你总是可以通过在交互式shell中进行输入来判断一条指令是否可以工作。不要担心弄坏电脑：能够发生的最坏的事情无非是Python反馈给你一条错误信息。专业的软件开发者在写代码的时候也总是会得到错误提示。</p>

<h2><a id="user-content-the-integer-floating-point-and-string-data-types" class="anchor" href="#the-integer-floating-point-and-string-data-types" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>The Integer, Floating-Point, and String Data Types</h2>

<h2><a id="user-content-整型浮点型和字符串类型" class="anchor" href="#整型浮点型和字符串类型" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>整型，浮点型和字符串类型</h2>

<p>Remember that expressions are just values combined with operators, and they always evaluate down to a single value. A data type is a category for values, and every value belongs to exactly one data type. The most common data types in Python are listed in Table 1-2. The values -2 and 30, for example, are said to be integer values. The integer (or int) data type indicates values that are whole numbers. Numbers with a decimal point, such as 3.14, are called floating-point numbers (or floats). Note that even though the value 42 is an integer, the value 42.0 would be a floating-point number.</p>

<p>记住，表达式仅仅是值和操作符的组合，而且它们总是会求出一个单一的值。数据类型说一个值的种类，所有的值都属于某一个特定的类型。Python中最常见的数据类型已经列在表1-2中。比如说，-2和30是整型。整型（或者int）类型表示一个值是整数。
带有小数点的值，比如3.14，被称之为浮点型（或float）。注意，即使42是一个整数，42.0会被看作是一个浮点值。</p>

<table><thead>
<tr>
<th align="center">Data type</th>
<th align="center">Examples</th>
</tr>
</thead><tbody>
<tr>
<td align="center">Integers</td>
<td align="center">-2, -1, 0, 1, 2, 3, 4, 5</td>
</tr>
<tr>
<td align="center">Floating-point numbers</td>
<td align="center">-1.25, -1.0, --0.5, 0.0, 0.5, 1.0, 1.25</td>
</tr>
<tr>
<td align="center">Strings</td>
<td align="center">'a', 'aa', 'aaa', 'Hello!', '11 cats'</td>
</tr>
</tbody></table>

<table><thead>
<tr>
<th align="center">数据类型</th>
<th align="center">示例</th>
</tr>
</thead><tbody>
<tr>
<td align="center">整型</td>
<td align="center">-2, -1, 0, 1, 2, 3, 4, 5</td>
</tr>
<tr>
<td align="center">浮点型</td>
<td align="center">-1.25, -1.0, --0.5, 0.0, 0.5, 1.0, 1.25</td>
</tr>
<tr>
<td align="center">字符串型</td>
<td align="center">'a', 'aa', 'aaa', 'Hello!', '11 cats'</td>
</tr>
</tbody></table>

<p>Python programs can also have text values called strings, or strs (pronounced “stirs”). Always surround your string in single quote (') characters (as in '<strong>Hello</strong>' or '<strong>Goodbye cruel world!</strong>') so Python knows where the string begins and ends. You can even have a string with no characters in it, '', called a blank string. Strings are explained in greater detail in Chapter 4.
If you ever see the error message <strong>SyntaxError: EOL while scanning string literal</strong>, you probably forgot the final single quote character at the end of the string, such as in this example:</p>

<p>Python程序也可以有一些文本值，叫做字符串，或者strs（读作“stirs”）。始终要用单引号（‘）来包裹你的字符串（就像'<strong>Hello</strong>' 或 '<strong>Goodbye cruel world!</strong>'），这样Python就知道了字符串的起始和结尾。你也可以创建没有字符的字符串，<code>''</code>，叫做空字符串。字符串将在第四章做详细介绍。
如果你曾经见过这样的错误信息：<strong>SyntaxError: EOL while scanning string literal</strong>，你可能是忘记了字符串的结束引号，比如例子中这样。</p>

<pre><code>&gt;&gt;&gt; 'Hello world!
SyntaxError: EOL while scanning string literal
</code></pre>

<h2><a id="user-content-string-concatenation-and-replication" class="anchor" href="#string-concatenation-and-replication" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>String Concatenation and Replication</h2>

<h2><a id="user-content-字符串连接与复制" class="anchor" href="#字符串连接与复制" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>字符串连接与复制</h2>

<p>The meaning of an operator may change based on the data types of the values next to it. For example, + is the addition operator when it operates on two integers or floating-point values. However, when + is used on two string values, it joins the strings as the string concatenation operator. Enter the following into the interactive shell:</p>

<p>操作符的意义可能会随着它后面的变量的类型而变化。比如说，<code>+</code>对于两个整数或是浮点数的意思是加号。然而，如果把它应用于两个字符串，它会把两个字符串链接起来，作为连接操作符。在交互式命令行里输入下面的代码：</p>

<pre><code>&gt;&gt;&gt; 'Alice' + 'Bob'
'AliceBob'
</code></pre>

<p>The expression evaluates down to a single, new string value that combines the text of the two strings. However, if you try to use the + operator on a string and an integer value, Python will not know how to handle this, and it will display an error message.</p>

<p>表达式求值得到单一的值，新的字符串把两个字符串的文本合并起来。然而，如果你尝试对一个字符串和一个整数使用＋号，Python就不知道如何应对了，它就会显示一条错误信息。</p>

<pre><code>&gt;&gt;&gt; 'Alice' + 42
Traceback (most recent call last):
  File "&lt;pyshell#26&gt;", line 1, in &lt;module&gt;
    'Alice' + 42
TypeError: Can't convert 'int' object to str implicitly
</code></pre>

<p>The error message <strong>Can't convert 'int' object to str implicitly</strong> means that Python thought you were trying to concatenate an integer to the string '<strong>Alice</strong>'. Your code will have to explicitly convert the integer to a string, because Python cannot do this automatically. (Converting data types will be explained in <a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/blob/lingfeng-ch2">Dissecting Your Program</a> when talking about the <code>str()</code>, <code>int()</code>, and <code>float()</code> functions.)</p>

<p>错误信息 <strong>Can't convert 'int' object to str implicitly</strong> 的意思是，Python认为你尝试把一个整数连接到字符串'<strong>Alice</strong>'。你的代码需要显式把整数转换为字符串，因为Python不能自动完成这一步。(数据类型转换将在<a href="/lisiyu/Automate-the-Boring-Stuff-with-Python-ChineseVersion/blob/lingfeng-ch2">Dissecting Your Program</a> 中解释，当我们谈到<code>str()</code>, <code>int()</code>, 和 <code>float()</code> 函数的时。)</p>

<pre><code>&gt;&gt;&gt; 'Alice' * 5
'AliceAliceAliceAliceAlice'
</code></pre>

<p>The expression evaluates down to a single string value that repeats the original a number of times equal to the integer value. String replication is a useful trick, but it’s not used as often as string concatenation.
The * operator can be used with only two numeric values (for multiplication) or one string value and one integer value (for string replication). Otherwise, Python will just display an error message.
表达式求值得到一个值，这个值把原始的字符串重复某个整数次。字符串复制是一个有用的技巧，但是它使用的次数并不如字符串连接那么多。＊操作符可以被用于两个数字值（做乘法）或者是一个字符串值和一个整数值（做字符串复制）。否则，Python会显示一条错误信息。</p>

<pre><code>&gt;&gt;&gt; 'Alice' * 'Bob'
Traceback (most recent call last):
  File "&lt;pyshell#32&gt;", line 1, in &lt;module&gt;
    'Alice' * 'Bob'
TypeError: can't multiply sequence by non-int of type 'str'
&gt;&gt;&gt; 'Alice' * 5.0
Traceback (most recent call last):
  File "&lt;pyshell#33&gt;", line 1, in &lt;module&gt;
    'Alice' * 5.0
TypeError: can't multiply sequence by non-int of type 'float'
</code></pre>

<p>It makes sense that Python wouldn’t understand these expressions: You can’t multiply two words, and it’s hard to replicate an arbitrary string a fractional number of times.</p>

<p>Python不能理解这些表达式是有道理的：你不能把两个单词相乘，而且也不能把一个任意的字符串复制非整数次。</p>

<h2><a id="user-content-storing-values-in-variables" class="anchor" href="#storing-values-in-variables" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Storing Values in Variables</h2>

<h2><a id="user-content-把值存放在变量中" class="anchor" href="#把值存放在变量中" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>把值存放在变量中</h2>

<p>A variable is like a box in the computer’s memory where you can store a single value. If you want to use the result of an evaluated expression later in your program, you can save it inside a variable.</p>

<p>变量就像是计算机内存中的一个盒子，你可以把一个值放在里面。如果你想在之后的程序中，使用一个表达式的结果，你可以把它存放在内部变量里。</p>

<h2><a id="user-content-assignment-statements" class="anchor" href="#assignment-statements" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Assignment Statements</h2>

<h2><a id="user-content-赋值语句" class="anchor" href="#赋值语句" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>赋值语句</h2>

<p>You’ll store values in variables with an assignment statement. An assignment statement consists of a variable name, an equal sign (called the assignment operator), and the value to be stored. If you enter the assignment statement spam = 42, then a variable named spam will have the integer value 42 stored in it.</p>

<p>你会通过复制语句来把值存入变量。一条复制语句包含一个变量名，一个等于号（被称作赋值号），和一个被储存的值。如果你输入赋值语句 spam=42,然后一个叫做spam的变量中就好存放一个整数值42。</p>

<p>Think of a variable as a labeled box that a value is placed in, as in Figure 1-2.
把一个变量想象为一个带标签的盒子，里面放有一个值，如图1-2所示。</p>

<p>For example, enter the following into the interactive shell:</p>

<p>比如，在交互式shell中输入下面命令：</p>

<pre><code>➊ &gt;&gt;&gt; spam = 40
   &gt;&gt;&gt; spam
   40
   &gt;&gt;&gt; eggs = 2
➋ &gt;&gt;&gt; spam + eggs
   42
   &gt;&gt;&gt; spam + eggs + spam
   82
➌ &gt;&gt;&gt; spam = spam + 2
   &gt;&gt;&gt; spam
   42
</code></pre>

<p>A variable is initialized (or created) the first time a value is stored in it ➊. After that, you can use it in expressions with other variables and values ➋. When a variable is assigned a new value ➌, the old value is forgotten, which is why spam evaluated to 42 instead of 40 at the end of the example. This is called overwriting the variable. Enter the following code into the interactive shell to try overwriting a string:</p>

<p>变量在第一次有值存入时被初始化（或创建）➊。这之后你就可以在表达式中使用它喝其他变量和值➋. 当一个变量被赋予新值时➌,旧的值就被忘记，这也是为什么在例子的最后，spam值为人42而不是40。这被称之为变量的覆盖。在交互式shell中输入下面的代码来尝试覆盖一个字符串:</p>

<pre><code>&gt;&gt;&gt; spam = 'Hello'
&gt;&gt;&gt; spam
'Hello'
&gt;&gt;&gt; spam = 'Goodbye'
&gt;&gt;&gt; spam
'Goodbye'  
</code></pre>

<p>Just like the box in Figure 1-3, the spam variable in this example stores 'Hello' until you replace it with 'Goodbye'.</p>

<p>就像图1-3中点盒子一样，本例中的spam变量存放了‘Hello',知道你用'Goodbye'覆盖了它。</p>

<h2><a id="user-content-variable-names" class="anchor" href="#variable-names" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Variable Names</h2>

<h2><a id="user-content-变量名" class="anchor" href="#变量名" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>变量名</h2>

<p>Table 1-3 has examples of legal variable names. You can name a variable anything as long as it obeys the following three rules:
表1-3列举了一些合法的变量名。只要符合以下三条规则，你可以任意命名你的变量：</p>

<ol>
<li>It can be only one word.</li>
<li>It can use only letters, numbers, and the underscore (_) character.</li>
<li><p>It can’t begin with a number. </p></li>
<li><p>它只能是一个单词。</p></li>
<li>它只能使用字母，数字合下划线（<code>_</code>）。</li>
<li>它不能以数字开头。</li>
</ol>

<table><thead>
<tr>
<th align="center">Valid variable names</th>
<th align="center">Invalid variable names</th>
</tr>
</thead><tbody>
<tr>
<td align="center">balance</td>
<td align="center">current-balance (hyphens are not allowed)</td>
</tr>
<tr>
<td align="center">currentBalance</td>
<td align="center"></td>
</tr>
<tr>
<td align="center">current_balance</td>
<td align="center">4account (can’t begin with a number)</td>
</tr>
<tr>
<td align="center">_spam</td>
<td align="center">42 (can’t begin with a number)</td>
</tr>
<tr>
<td align="center">SPAM</td>
<td align="center">total_$um (special characters like $ are not allowed)</td>
</tr>
<tr>
<td align="center">account4</td>
<td align="center">'hello' (special characters like ' are not allowed)</td>
</tr>
</tbody></table>

<table><thead>
<tr>
<th align="center">有效变量名</th>
<th align="center">无效变量名</th>
</tr>
</thead><tbody>
<tr>
<td align="center">balance</td>
<td align="center">current-balance (<code>-</code>不允许使用)</td>
</tr>
<tr>
<td align="center">currentBalance</td>
<td align="center"></td>
</tr>
<tr>
<td align="center">current_balance</td>
<td align="center">4account (不能以数字开头)</td>
</tr>
<tr>
<td align="center">_spam</td>
<td align="center">42 (不能以数字开头)</td>
</tr>
<tr>
<td align="center">SPAM</td>
<td align="center">total_$um (像<code>$</code>这样的特殊字符不允许)</td>
</tr>
<tr>
<td align="center">account4</td>
<td align="center">'hello' (像<code>'</code>这样的特殊字符不允许)</td>
</tr>
</tbody></table>

<p>Variable names are case-sensitive, meaning that <strong>spam</strong>, <strong>SPAM</strong>, <strong>Spam</strong>, and <strong>sPaM</strong> are four different variables. It is a Python convention to start your variables with a lowercase letter.
This book uses camelcase for variable names instead of underscores; that is, variables <strong>lookLikeThis</strong> instead of <strong>looking_like_this</strong>. Some experienced programmers may point out that the official Python code style, PEP 8, says that underscores should be used. I unapologetically prefer camelcase and point to “A Foolish Consistency Is the Hobgoblin of Little Minds” in PEP 8 itself:</p>

<p>变量名区分大小写，这意味着<strong>spam</strong>, <strong>SPAM</strong>, <strong>Spam</strong>, 和<strong>sPaM</strong> 是四个不同的变量名。变量名以小写字母开头是Python的惯例。</p>

<p>本书使用驼峰命名法，而不是下划线；也就是说，使用<strong>lookLikeThis</strong> 而不是<strong>looking_like_this</strong>。一些有经验的程序员也许会指出，官方Python代码风格PEP8认为应当使用下划线。我仍不知错的要，使用驼峰命名法，并指出PEP8中“愚蠢的一致性就像没有脑子的妖怪”一节所说：</p>

<blockquote>
<p>“Consistency with the style guide is important. But most importantly: know when to be inconsistent—sometimes the style guide just doesn’t apply. When in doubt, use your best judgment.”</p>

<p>“与风格指南保持一致是很重要的。但是更重要的是：知道何时变的不一致——有些时候风格指南就是不适用。当你有所怀疑的时候，相信自己最好的判断”</p>
</blockquote>

<p>A good variable name describes the data it contains. Imagine that you moved to a new house and labeled all of your moving boxes as Stuff. You’d never find anything! The variable names spam, eggs, and bacon are used as generic names for the examples in this book and in much of Python’s documentation (inspired by the Monty Python “Spam” sketch), but in your programs, a descriptive name will help make your code more readable.</p>

<p>一个好的变量名描述了它所存放的变量。想象着你搬进了一个新家，然后把你所有搬来的包裹都贴上了“东西”这个标签。那你就永远无法找到任何东西了！变量名spam, eggs, 还有 bacon，在本书的例子中以及Python文档中作为几个通用变量名。（受到Monty Python短剧“spam”短剧的启发），但是在你的程序中，一个描述性的名字会让你的程序更加易读。</p>

<h2><a id="user-content-your-first-program" class="anchor" href="#your-first-program" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Your First Program</h2>

<h2><a id="user-content-你的第一个程序" class="anchor" href="#你的第一个程序" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>你的第一个程序</h2>

<p>While the interactive shell is good for running Python instructions one at a time, to write entire Python programs, you’ll type the instructions into the file editor. The file editor is similar to text editors such as Notepad or TextMate, but it has some specific features for typing in source code. To open the file editor in IDLE, select File▸New Window.
The window that appears should contain a cursor awaiting your input, but it’s different from the interactive shell, which runs Python instructions as soon as you press ENTER. The file editor lets you type in many instructions, save the file, and run the program. Here’s how you can tell the difference between the two:</p>

<p>尽管交互式shell很适合一次运行一条Python指令，为了写一个完整的程序，你还是会把程序输入到文件编辑器中。文件编辑器和文本编辑器类似，比如Notepad或是TextMate，但是它对于输入源代码具有一些特殊的功能。在IDLE中打开文件编辑器，选择File▸New Window。新打开的窗口中应该有一个等待你输入的光标,但是和交互式命令行有一些不同，交互式命令行在你按下回车后立即执行。文件编辑器允许你输入多项命令，保存文件，然后运行程序。以下是你如何分辨二者：</p>

<ul>
<li>The interactive shell window will always be the one with the <code>&gt;&gt;&gt;</code>prompt.</li>
<li><p>The file editor window will not have the <code>&gt;&gt;&gt;</code>prompt.</p></li>
<li><p>交互式shell窗口总是有<code>&gt;&gt;&gt;</code>的那一个。</p></li>
<li>文件编辑器是没有<code>&gt;&gt;&gt;</code>的那一个。</li>
</ul>

<p>Now it’s time to create your first program! When the file editor window opens, type the following into it:</p>

<p>现在，是时候创建你的第一个程序了！当文件编辑器开启后，输入如下命令：</p>

<pre><code>➊ # This program says hello and asks for my name.
➋ print('Hello world!')
   print('What is your name?')    # ask for their name
➌ myName = input()
➍ print('It is good to meet you, ' + myName)
➎ print('The length of your name is:')
   print(len(myName))
➏ print('What is your age?')    # ask for their age
   myAge = input()
   print('You will be ' + str(int(myAge) + 1) + ' in a year.')
</code></pre>

<p>Once you’ve entered your source code, save it so that you won’t have to retype it each time you start IDLE. From the menu at the top of the file editor window, select File▸Save As. In the Save As window, enter <strong>hello.py</strong> in the File Name field and then click Save.
一旦你输入完成源代码，把它保存下来这样你就不需要在每一次启动IDLE时重复输入了。在文件编辑器顶端的菜单里面选择 File▸Save As。在保存窗口中文件名一栏输入 <strong>hello.py</strong> 然后点击保存。</p>

<p>You should save your programs every once in a while as you type them. That way, if the computer crashes or you accidentally exit from IDLE, you won’t lose the code. As a shortcut, you can press CTRL-S on Windows and Linux or ⌘-S on OS X to save your file.
当你输入一段时间后，就应该保存你的程序。这样的话，如果电脑死机了或是你不小心退出了IDLE，你不会丢失代码。说到快捷键，你可以在Windows 和 Linux上用CTRL-S或者在OS X上使用⌘-S来保存文件。 </p>

<p>Once you’ve saved, let’s run our program. Select Run▸Run Module or just press the F5 key. Your program should run in the interactive shell window that appeared when you first started IDLE. Remember, you have to press F5 from the file editor window, not the interactive shell window. Enter your name when your program asks for it. The program’s output in the interactive shell should look something like this:</p>

<p>一旦你完成保存，让我们运行我们的程序。选择 Run▸Run Module或按F5键。你的程序会在你第一次打开的交互式shell窗口中运行。记住，你需要在文件编辑器中按下F5，而不是交互式shell中。当程序像你询问时，输入你的名字。交互式命令行中会显示下面的内容：</p>

<pre><code>Python 3.3.2 (v3.3.2:d047928ae3f6, May 16 2013, 00:06:53) [MSC v.1600 64 bit
(AMD64)] on win32
Type "copyright", "credits" or "license()" for more information.
&gt;&gt;&gt; ================================ RESTART ================================
&gt;&gt;&gt;
Hello world!
What is your name?
Al
It is good to meet you, Al
The length of your name is:
2
What is your age?
4
You will be 5 in a year.
&gt;&gt;&gt;
</code></pre>

<p>When there are no more lines of code to execute, the Python program terminates; that is, it stops running. (You can also say that the Python program <em>exits</em>.)
You can close the file editor by clicking the X at the top of the window. To reload a saved program, select File▸Open from the menu. Do that now, and in the window that appears, choose hello.py, and click the Open button. Your previously saved hello.py program should open in the file editor window.</p>

<p>当没有代码需要被执行打时候，Python程序就终止了；意思是，停止运行。（你同样也可以说Python程序<strong>退出</strong>(exit)了。）
你可以点击窗口上方的X来关闭文件编辑器。要重新载入一个保存过的程序，在菜单中选择File▸Open。现在就试一下，并且当有窗口弹出的时候，选择hello.py，然后点击打开按钮。
你之前保存的hello.py文件应该会出现在文件编辑器窗口中。</p>

<h2><a id="user-content-dissecting-your-program" class="anchor" href="#dissecting-your-program" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Dissecting Your Program</h2>

<h2><a id="user-content-剖析你的程序" class="anchor" href="#剖析你的程序" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>剖析你的程序</h2>

<p>With your new program open in the file editor, let’s take a quick tour of the Python instructions it uses by looking at what each line of code does.</p>

<p>对你在文件编辑器中打开的文件，让我们通过观察各行代码来快速浏览一下这个程序所用到的Python指令。</p>

<h3><a id="user-content-comments" class="anchor" href="#comments" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Comments</h3>

<h3><a id="user-content-注释" class="anchor" href="#注释" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>注释</h3>

<p>The following line is called a comment.
下面这一行叫做注释。</p>

<pre><code>➊ # This program says hello and asks for my name.
</code></pre>

<p>Python ignores comments, and you can use them to write notes or remind yourself what the code is trying to do. Any text for the rest of the line following a hash mark (#) is part of a comment.</p>

<p>Python会忽略注释，你可以利用注释来做笔记或提醒你这段代码要做的事情。#号后面所有的文本都被看作是注释的一部分。</p>

<p>Sometimes, programmers will put a # in front of a line of code to temporarily remove it while testing a program. This is called commenting out code, and it can be useful when you’re trying to figure out why a program doesn’t work. You can remove the # later when you are ready to put the line back in.</p>

<p>有时候，当程序员们测试程序的时候，会在某行代码前加一个#将这行代码临时移除。我们称之为，注释掉（comment out）代码，在你想要搞明白程序为什么不工作的时候，这是非常有用大。当你准备把这行重新加入的时候，你可以把#号移除。</p>

<p>Python also ignores the blank line after the comment. You can add as many blank lines to your program as you want. This can make your code easier to read, like paragraphs in a book.</p>

<h3><a id="user-content-the-print-function" class="anchor" href="#the-print-function" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>The print() Function</h3>

<h3><a id="user-content-print函数" class="anchor" href="#print函数" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>print()函数</h3>

<p><g-emoji alias="two" fallback-src="https://assets-cdn.github.com/images/icons/emoji/unicode/0032-20e3.png">2⃣️</g-emoji><strong>译注：关于Python 2和Python 3的print函数用法不同，可以参考这个<a href="http://www.python-course.eu/python3_print.php">链接</a></strong></p>

<p>The print() function displays the string value inside the parentheses on the screen.
print()函数会吧括号内的字符串显示在屏幕上。</p>

<pre><code>➋ print('Hello world!')
   print('What is your name?') # ask for their name
</code></pre>

<p>The line <strong>print('Hello world!')</strong> means “Print out the text in the string '<strong>Hello world!</strong>'.” When Python executes this line, you say that Python is calling the <strong>print()</strong> function and the string value is being passed to the function. A value that is passed to a function call is an argument. Notice that the quotes are not printed to the screen. They just mark where the string begins and ends; they are not part of the string value.</p>

<p><strong>print('Hello world!')</strong>这行代码的意思是“打印字符串中的文本‘<strong>Hello world!</strong>’。”当Python执行这一行的时候，你可以说Python调用了<strong>print()</strong>函数，同时字符串对值被传入了函数。传入函数的值我们称之为参数。注意引号并不会被打印在屏幕上。它仅仅标记了字符串的起点和结束；它们并不是字符串的一部分。</p>

<p><strong>NOTE</strong>
<em>You can also use this function to put a blank line on the screen; just call print() with nothing in between the parentheses.</em></p>

<p><strong>注意</strong>
<em>你同样可以用这个函数在屏幕上输出一个空行；调用print()，括号里面什么都没有，就可以了。</em></p>

<p>When writing a function name, the opening and closing parentheses at the end identify it as the name of a function. This is why in this book you’ll see print() rather than print. Chapter 2 describes functions in more detail.
当写下一个函数的名字时，它后面的括号会使它成为函数名。这也是为什么你在本书中会看到print()而不是print。第二章更加详细的描述了函数。</p>

<h3><a id="user-content-the-input-function" class="anchor" href="#the-input-function" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>The input() Function</h3>

<h3><a id="user-content-input函数" class="anchor" href="#input函数" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>input()函数</h3>

<p>The input() function waits for the user to type some text on the keyboard and press ENTER.
input()函数等待用户从键盘输入一些文本，并按下回车。</p>

<pre><code>➌ myName = input()
</code></pre>

<p>This function call evaluates to a string equal to the user’s text, and the previous line of code assigns the myName variable to this string value.
这个函数求值得到一个字符串，等同于用户输入的文本，前面一部分代码把变量名myName赋给这个字符串值。</p>

<p>You can think of the <strong>input()</strong> function call as an expression that evaluates to whatever string the user typed in. If the user entered 'Al', then the expression would evaluate to <strong>myName = 'Al'</strong>.</p>

<p>你可以认为<strong>input()</strong>被当作一个表达式调用，并且它求值得到的结果是用户输入的任何字符串。如果用户输入'Al'，那么这个表达式的值就是<strong>myName = 'Al'</strong>。</p>

<h3><a id="user-content-printing-the-users-name" class="anchor" href="#printing-the-users-name" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Printing the User’s Name</h3>

<p>The following call to print() actually contains the expression '<strong>It is good to meet you, ' + myName</strong> between the parentheses.</p>

<pre><code>➍ print('It is good to meet you, ' + myName)
</code></pre>

<p>Remember that expressions can always evaluate to a single value. If 'Al' is the value stored in myName on the previous line, then this expression evaluates to '<strong>It is good to meet you, Al</strong>'. This single string value is then passed to print(), which prints it on the screen.</p>

<p>记住，表达式总是会求得唯一多值。如果'Al'是前面一行代码保存在myName中的值，那么这个表达式求值得到'<strong>It is good to meet you, Al</strong>'，这个单一的字符串随之被传给print()，它会把字符串打印到屏幕上。</p>

<h3><a id="user-content-the-len-function" class="anchor" href="#the-len-function" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>The len() Function</h3>

<h3><a id="user-content-len函数" class="anchor" href="#len函数" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>len()函数</h3>

<p>You can pass the len() function a string value (or a variable containing a string), and the function evaluates to the integer value of the number of characters in that string.
你可以向len()函数传递一个字符串值（或是一个包含字符串的变量），这个函数会求值得到代表这个字符串中字符个数的一个整数值。</p>

<pre><code>➎ print('The length of your name is:')
  print(len(myName))
</code></pre>

<p>Enter the following into the interactive shell to try this:
在交互式命令行里面输入下面代码：</p>

<pre><code>&gt;&gt;&gt; len('hello')
5
&gt;&gt;&gt; len('My very energetic monster just scarfed nachos.')
46
&gt;&gt;&gt; len('')
0
</code></pre>

<p>Just like those examples, len(myName) evaluates to an integer. It is then passed to print() to be displayed on the screen. Notice that print() allows you to pass it either integer values or string values. But notice the error that shows up when you type the following into the interactive shell:</p>

<p>就像这些例子一样，<code>len(myName)</code>求值得到一个整数，然后它被传递给print()用以显示在屏幕上。注意print()允许你传递整数或者字符串。但是，当你在交互式命令行中输入如下命令的时候，请注意显示到错误信息。</p>

<pre><code>&gt;&gt;&gt; print('I am ' + 29 + ' years old.')
Traceback (most recent call last):
  File "&lt;pyshell#6&gt;", line 1, in &lt;module&gt;
    print('I am ' + 29 + ' years old.')
TypeError: Can't convert 'int' object to str implicitly
</code></pre>

<p>The <strong>print()</strong> function isn’t causing that error, but rather it’s the expression you tried to pass to print(). You get the same error message if you type the expression into the interactive shell on its own.</p>

<p>并不是<strong>print()</strong>引起了错误，而是你传递进print()的表达式。你把这个表达式单独输入交互式命令后，也会得到同样的错误信息。</p>

<pre><code>&gt;&gt;&gt; 'I am ' + 29 + ' years old.'
Traceback (most recent call last):
  File "&lt;pyshell#7&gt;", line 1, in &lt;module&gt;
    'I am ' + 29 + ' years old.'
TypeError: Can't convert 'int' object to str implicitly
</code></pre>

<p>Python gives an error because you can use the + operator only to add two integers together or concatenate two strings. You can’t add an integer to a string because this is ungrammatical in Python. You can fix this by using a string version of the integer instead, as explained in the next section.</p>

<p>Python输出了一条错误信息，因为你只可以用+操作符把两个整数相加或是连接两个字符串。你不能把一个整数和一个字符串相加，因为这不符合Python语法。你可以可以使用这个整数的字符串版本来修复这个问题，就像我们下一节将要讲的那样。</p>

<h3><a id="user-content-the-str-int-and-float-functions" class="anchor" href="#the-str-int-and-float-functions" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>The str(), int(), and float() Functions</h3>

<h3><a id="user-content-str-int和float函数" class="anchor" href="#str-int和float函数" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>str(), int(),和float()函数</h3>

<p>If you want to concatenate an integer such as 29 with a string to pass to print(), you’ll need to get the value '29', which is the string form of 29. The str() function can be passed an integer value and will evaluate to a string value version of it, as follows:</p>

<p>如果你想要把一个整数，例如29和一个字符串连接起来传入print()函数，你需要得到'29'这个值，它是29的字符串形式。str()函数可以传入一个整数值并且会求得它的一个字符串版本，就像下面这样：</p>

<pre><code>&gt;&gt;&gt; str(29)
'29'
&gt;&gt;&gt; print('I am ' + str(29) + ' years old.')
I am 29 years old.
</code></pre>

<p>Because str(29) evaluates to '29', the expression 'I am ' + str(29) + ' years old.' evaluates to 'I am ' + '29' + ' years old.', which in turn evaluates to 'I am 29 years old.'. This is the value that is passed to the print() function.</p>

<p>因为str(29)求值得到‘29’，表达式'I am ' + str(29) + ' years old .'求值得到'I am ' + '29' + ' years old.'，随后求值得到'I am 29 years old.'。这就是传入print()的值。</p>

<p>The str(), int(), and float() functions will evaluate to the string, integer, and floating-point forms of the value you pass, respectively. Try converting some values in the interactive shell with these functions, and watch what happens.
str(), int(),和float()函数会分别求值得出传入值的字符串，整型，和浮点型版本。在交互式shell中尝试使用这些函数来转换一些值，看看会发生什么？</p>

<pre><code>&gt;&gt;&gt; str(0)
'0'
&gt;&gt;&gt; str(-3.14)
'-3.14'
&gt;&gt;&gt; int('42')
42
&gt;&gt;&gt; int('-99')
-99
&gt;&gt;&gt; int(1.25)
1
&gt;&gt;&gt; int(1.99)
1
&gt;&gt;&gt; float('3.14')
3.14
&gt;&gt;&gt; float(10)
10.0
</code></pre>

<p>The previous examples call the str(), int(), and float() functions and pass them values of the other data types to obtain a string, integer, or floating-point form of those values.
前面的代码调用了str(), int(), 以及float()函数，并且向他们传递其他的数据类型，来得到它们字符串，整型或是浮点型版本。</p>

<p>The str() function is handy when you have an integer or float that you want to concatenate to a string. The int() function is also helpful if you have a number as a string value that you want to use in some mathematics. For example, the input() function always returns a string, even if the user enters a number. Enter <strong>spam = input()</strong> into the interactive shell and enter <strong>101</strong> when it waits for your text.</p>

<p>当你想要把一个整型或浮点型数与字符串相连时，str()函数非常方便好用。当你想要用一个字符串类型的数做数学运算的时候，int()函数同样很有用。例如，input()函数总是返回一个字符串，即使你输入的是一个数字。在交互式shell中输入<strong>spam = input()</strong>，并且在当它等待你输入时，输入<strong>101</strong>。</p>

<pre><code>&gt;&gt;&gt; spam = input()
101
&gt;&gt;&gt; spam
'101'
</code></pre>

<p>The value stored inside spam isn’t the integer 101 but the string '101'. If you want to do math using the value in spam, use the int() function to get the integer form of spam and then store this as the new value in spam.
存放在spam变量中的值并不是整型的101。而是字符串‘101’。如果你先要用这个值做数学运算，使用int()函数来获取spam的整型版本，并把它作为一个新的值存放在spam中。</p>

<pre><code>&gt;&gt;&gt; spam = int(spam)
&gt;&gt;&gt; spam
101
</code></pre>

<p>Now you should be able to treat the spam variable as an integer instead of a string.</p>

<p>现在，你可以把spam看作一个整型而不是字符串了。</p>

<pre><code>&gt;&gt;&gt; spam * 10 / 5
202.0
</code></pre>

<p>Note that if you pass a value to int() that it cannot evaluate as an integer, Python will display an error message.</p>

<p>注意到如果你把一个不可以转换为整数的值传递给int()，Python会显示一条错误信息。</p>

<pre><code>&gt;&gt;&gt; int('99.99')
Traceback (most recent call last):
  File "&lt;pyshell#18&gt;", line 1, in &lt;module&gt;
    int('99.99')
ValueError: invalid literal for int() with base 10: '99.99'
&gt;&gt;&gt; int('twelve')
Traceback (most recent call last):
  File "&lt;pyshell#19&gt;", line 1, in &lt;module&gt;
    int('twelve')
ValueError: invalid literal for int() with base 10: 'twelve'
</code></pre>

<p>The int() function is also useful if you need to round a floating-point number down. If you want to round a floating-point number up, just add 1 to it afterward.</p>

<p>如果你想要对一个浮点数进行向下取整，int()函数同样很有用，如果想进行向上取整，只需要紧接着加1即可。</p>

<pre><code>&gt;&gt;&gt; int(7.7)
7
&gt;&gt;&gt; int(7.7) + 1
8
</code></pre>

<p>In your program, you used the int() and str() functions in the last three lines to get a value of the appropriate data type for the code.
在你的程序中，你在最后三行使用int()和str()函数来获取代码所需要的合适的数据类型。</p>

<pre><code>➏ print('What is your age?') # ask for their age
   myAge = input()
   print('You will be ' + str(int(myAge) + 1) + ' in a year.')
</code></pre>

<p>The myAge variable contains the value returned from input(). Because the input() function always returns a string (even if the user typed in a number), you can use the int(myAge) code to return an integer value of the string in myAge. This integer value is then added to 1 in the expression int(myAge) + 1.</p>

<p>myAge变量包含了从input()返回的值。因为input()函数总是返回一个字符串（即使你输入了一个数字），你可以使用int(myAge)来返回myAge中字符串的整数值。这个整数值随后在表达式int(myAge)+1中被加1。</p>

<p>The result of this addition is passed to the str() function: str(int(myAge) + 1). The string value returned is then concatenated with the strings 'You will be ' and ' in a year.' to evaluate to one large string value. This large string is finally passed to print() to be displayed on the screen.
这次相加的结果被传递给str()函数：str(int(myAge) + 1)。函数返回的字符串随后与'You will be '和' in a year.'连接得到一个更长的字符串。这个字符串最终被传递给print()函数，来显示在屏幕上。</p>

<p>Let’s say the user enters the string '4' for myAge. The string '4' is converted to an integer, so you can add one to it. The result is 5. The str() function converts the result back to a string, so you can concatenate it with the second string, 'in a year.', to create the final message. These evaluation steps would look something like Figure 1-4.</p>

<p>让我们假设用户输入了字符串'4'作为年龄。字符串'4'会被转换为一个整型，所以你可以对其＋1。str()函数把结果转换回字符串，所以你可以把它喝第二个字符串'in a year.'得到最终消息。求值步骤看上去像图1-4表示的那样。</p>

<h2><a id="user-content-summary" class="anchor" href="#summary" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Summary</h2>

<h2><a id="user-content-总结" class="anchor" href="#总结" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>总结</h2>

<p>You can compute expressions with a calculator or type string concatenations with a word processor. You can even do string replication easily by copying and pasting text. But expressions, and their component values—operators, variables, and function calls—are the basic building blocks that make programs. Once you know how to handle these elements, you will be able to instruct Python to operate on large amounts of data for you.</p>

<p>你可以使用计算器来求解表达式或者用词处理器来连接输入的字符串。你甚至可以通过复制粘贴文本来复制字符串。但是，表达式，以及它们的组成部分值－操作符，变量和函数调用是构建程序的基础素材。一旦你了解了如何处理这些元素，你就可以命令Python来为你操作大量的数据。</p>

<p>It is good to remember the different types of operators (+, -, <em>, /, //, %, and *</em> for math operations, and + and * for string operations) and the three data types (integers, floating-point numbers, and strings) introduced in this chapter.</p>

<p>记住本章介绍的不同类型的操作符 (+, -, <em>, /, //, %, 和 *</em> 这些算数操作符,以及 + 和 * 这样的字符串操作符) 以及三种数据类型 (整型, 浮点型, 和字符串)是有益的。</p>

<p>A few different functions were introduced as well. The print() and input() functions handle simple text output (to the screen) and input (from the keyboard). The len() function takes a string and evaluates to an int of the number of characters in the string. The str(), int(), and float() functions will evaluate to the string, integer, or floating-point number form of the value they are passed.</p>

<p>同时还介绍了一些不同的函数。print() 和 input()函数处理简单的输出 (到屏幕)和输入(从键盘)。 len()函数获取一个字符串，求出字符串中包含字符的整型值。str(), int(), 和float()函数会得到传入值的字符串型，整型和浮点型值。</p>

<p>In the next chapter, you will learn how to tell Python to make intelligent decisions about what code to run, what code to skip, and what code to repeat based on the values it has. This is known as flow control, and it allows you to write programs that make intelligent decisions.</p>

<p>在下一章中，你会学习如何让Python做出智能的判断，决定该执行哪些代码，跳过哪些代码以及哪些代码需要基于某个值重复执行。这些被称作流控制（flow control），它允许你写出可以进行智能决断的程序。</p>

<h2><a id="user-content-practice-questions" class="anchor" href="#practice-questions" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>Practice Questions</h2>

<h2><a id="user-content-练习问题" class="anchor" href="#练习问题" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1h-1c-1.5 0-3-1.69-3-3.5s1.55-3.5 3-3.5h4c1.45 0 3 1.69 3 3.5 0 1.41-0.91 2.72-2 3.25v-1.16c0.58-0.45 1-1.27 1-2.09 0-1.28-1.02-2.5-2-2.5H4c-0.98 0-2 1.22-2 2.5s1 2.5 2 2.5z m9-3h-1v1h1c1 0 2 1.22 2 2.5s-1.02 2.5-2 2.5H9c-0.98 0-2-1.22-2-2.5 0-0.83 0.42-1.64 1-2.09v-1.16c-1.09 0.53-2 1.84-2 3.25 0 1.81 1.55 3.5 3 3.5h4c1.45 0 3-1.69 3-3.5s-1.5-3.5-3-3.5z"></path></svg></a>练习问题</h2>

<p>Q:
1. Which of the following are operators, and which are values?<br>
1. 下面哪些是操作符，哪些是值？</p>

<pre><code>*
'hello'
-88.8
-
/
+
5
</code></pre>

<p>Q:
2. Which of the following is a variable, and which is a string?<br>
2. 下面哪个是变量，哪个是字符串？</p>

<pre><code>spam
'spam'
</code></pre>

<p>Q:
3. Name three data types.<br>
3. 指出三种数据类型。</p>

<p>Q:
4. What is an expression made up of? What do all expressions do?<br>
4. 表达式由什么组成？所以的表达式都在做些什么？</p>

<p>Q:
5. This chapter introduced assignment statements, like spam = 10. What is the difference between an expression and a statement?<br>
5. 本章介绍了赋值语句，例如spam = 10，表达式和语句的区别是什么？</p>

<p>Q:
6. What does the variable bacon contain after the following code runs?<br>
6. 下面这段代码执行后变量bacon中的值是什么？  </p>

<pre><code>bacon = 20
bacon + 1
</code></pre>

<p>Q:
7. What should the following two expressions evaluate to?<br>
7.下面这两个表达式求值是什么？  </p>

<pre><code>'spam' + 'spamspam'
'spam' * 3
</code></pre>

<p>Q:
8. Why is eggs a valid variable name while 100 is invalid?<br>
8. 为什么100不是合法变量名，egg却是合法的？</p>

<p>Q:
9. What three functions can be used to get the integer, floating-point number, or string version of a value?<br>
9. 那三个函数可以被用来获取一个值的整型，浮点型数或是字符串版本？</p>

<p>Q:
10. Why does this expression cause an error? How can you fix it?<br>
10. 为什么下面表达式会引起错误？如何修改？   </p>

<pre><code>'I have eaten ' + 99 + ' burritos.'
</code></pre>

<p>Extra credit: Search online for the Python documentation for the len() function. It will be on a web page titled “Built-in Functions.” Skim the list of other functions Python has, look up what the round() function does, and experiment with it in the interactive shell.  </p>

<p>加分题：在网上搜索Python文档关于len()函数的内容。它会出现在一个叫做“Built-in Functions.” 的页面里。浏览一下列出的其他Python函数，查看round()是做什么的，并且在交互式命令后里面测试它。</p>
</article>
  </div>

</div>

<button type="button" data-facebox="#jump-to-line" data-facebox-class="linejump" data-hotkey="l" class="hidden">Jump to Line</button>
<div id="jump-to-line" style="display:none">
  <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

  </div>
  <div class="modal-backdrop"></div>
</div>


    </div>
  </div>

    </div>

        <div class="container site-footer-container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>
          <li><a href="https://github.com/pricing" data-ga-click="Footer, go to pricing, text:pricing">Pricing</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage" class="site-footer-mark">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" role="img" title="GitHub " version="1.1" viewBox="0 0 16 16" width="24"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59 0.4 0.07 0.55-0.17 0.55-0.38 0-0.19-0.01-0.82-0.01-1.49-2.01 0.37-2.53-0.49-2.69-0.94-0.09-0.23-0.48-0.94-0.82-1.13-0.28-0.15-0.68-0.52-0.01-0.53 0.63-0.01 1.08 0.58 1.23 0.82 0.72 1.21 1.87 0.87 2.33 0.66 0.07-0.52 0.28-0.87 0.51-1.07-1.78-0.2-3.64-0.89-3.64-3.95 0-0.87 0.31-1.59 0.82-2.15-0.08-0.2-0.36-1.02 0.08-2.12 0 0 0.67-0.21 2.2 0.82 0.64-0.18 1.32-0.27 2-0.27 0.68 0 1.36 0.09 2 0.27 1.53-1.04 2.2-0.82 2.2-0.82 0.44 1.1 0.16 1.92 0.08 2.12 0.51 0.56 0.82 1.27 0.82 2.15 0 3.07-1.87 3.75-3.65 3.95 0.29 0.25 0.54 0.73 0.54 1.48 0 1.07-0.01 1.93-0.01 2.2 0 0.21 0.15 0.46 0.55 0.38C13.71 14.53 16 11.53 16 8 16 3.58 12.42 0 8 0z"></path></svg>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2016 <span title="0.09635s from github-fe135-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>
    </ul>
  </div>
</div>



    
    
    

    <div id="ajax-error-message" class="ajax-error-message flash flash-error">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M15.72 12.5l-6.85-11.98C8.69 0.21 8.36 0.02 8 0.02s-0.69 0.19-0.87 0.5l-6.85 11.98c-0.18 0.31-0.18 0.69 0 1C0.47 13.81 0.8 14 1.15 14h13.7c0.36 0 0.69-0.19 0.86-0.5S15.89 12.81 15.72 12.5zM9 12H7V10h2V12zM9 9H7V5h2V9z"></path></svg>
      <button type="button" class="flash-close js-flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
        <svg aria-hidden="true" class="octicon octicon-x" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75-1.48-1.48 3.75-3.75L0.77 4.25l1.48-1.48 3.75 3.75 3.75-3.75 1.48 1.48-3.75 3.75z"></path></svg>
      </button>
      Something went wrong with that request. Please try again.
    </div>


      
      <script crossorigin="anonymous" integrity="sha256-5nfyAipdNuj1rTXQ/LAfg/HNthPtoESfUzGXaTvMa9o=" src="https://assets-cdn.github.com/assets/frameworks-e677f2022a5d36e8f5ad35d0fcb01f83f1cdb613eda0449f533197693bcc6bda.js"></script>
      <script async="async" crossorigin="anonymous" integrity="sha256-IpQVLDsKYwg78vtdTNQkL3QfAkD0LZvg030MJtRIoLQ=" src="https://assets-cdn.github.com/assets/github-2294152c3b0a63083bf2fb5d4cd4242f741f0240f42d9be0d37d0c26d448a0b4.js"></script>
      
      
      
      
    <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner hidden">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" role="img" version="1.1" viewBox="0 0 16 16" width="16"><path d="M15.72 12.5l-6.85-11.98C8.69 0.21 8.36 0.02 8 0.02s-0.69 0.19-0.87 0.5l-6.85 11.98c-0.18 0.31-0.18 0.69 0 1C0.47 13.81 0.8 14 1.15 14h13.7c0.36 0 0.69-0.19 0.86-0.5S15.89 12.81 15.72 12.5zM9 12H7V10h2V12zM9 9H7V5h2V9z"></path></svg>
      <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
      <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
    </div>
    <div class="facebox" id="facebox" style="display:none;">
  <div class="facebox-popup">
    <div class="facebox-content" role="dialog" aria-labelledby="facebox-header" aria-describedby="facebox-description">
    </div>
    <button type="button" class="facebox-close js-facebox-close" aria-label="Close modal">
      <svg aria-hidden="true" class="octicon octicon-x" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path d="M7.48 8l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75-1.48-1.48 3.75-3.75L0.77 4.25l1.48-1.48 3.75 3.75 3.75-3.75 1.48 1.48-3.75 3.75z"></path></svg>
    </button>
  </div>
</div>

  </body>
</html>

