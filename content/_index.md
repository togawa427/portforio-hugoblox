---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: 
    "2rem"
    # padding: [10, 10, 10, 10]
  

sections:
  - block: my-resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          # filename: stacked-waves-yellow.svg
          filename: mountsky.jpg
          #filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  # - block: markdown
  #   content:
  #     title: 'News'
  #     subtitle: ''
  #     # text: |-
  #     #   Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.

  #     #   I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.
        
  #     #   Please reach out to collaborate 😃
  #   design:
  #     columns: '1'

  # ニュース
  - block: collection
    id: news
    content:
      title: News
      subtitle: 'ニュース'
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [10, 0, 0, 0]

  # 経歴
  - block: my-resume-experience
    id: experience
    content:
      username: admin
    design:
      css_class: "bg-gray-100"
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
      spacing:
        padding: [10, 0, 0, 0]

  # スキル
  - block: my-resume-skills
    id: skills
    content:
      title: Skills
      username: admin
    design:
      show_skill_percentage: false
      spacing:
        padding: [10, 0, 0, 0]
  
  # 職務経歴
  - block: works
    id: work
    content:
      title: Works
      username: work
    design:
      css_class: "bg-gray-100"
      spacing:
        padding: [10, 0, 0, 0]
  # - block: resume-skills
  #   id: work
  #   content: 
  #     title: Work
  #     username: admin
  #   design:
  #     show_skill_percentage: false
  #     css_class: "bg-gray-100"

  # 開発物
  - block: collection
    id: products
    content:
      count: 100
      title: Products & Development
      # text: I enjoy making things. Here are a selection of projects that I have worked on over the years.
      filters:
        folders:
          - project
    design:
      view: article-grid
      fill_image: false
      columns: 3
      spacing:
        padding: [10, 0, 0, 0]

  # 発表実績
  - block: resume-awards
    id: events
    content:
      title: Events
      username: event
    design:
      css_class: "bg-gray-100"
      spacing:
        padding: [10, 0, 0, 0]
  
  # - block: collection
  #   id: events
  #   content:
  #     title: Events
  #     subtitle: '発表実績'
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: event
  #     # Choose how many pages you would like to display (0 = all pages)
  #     # Filter on criteria
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     css_class: "bg-gray-100"
  #     # Choose a layout view
  #     view: date-title-summary

  # 出版物      
  # - block: collection
  #   id: papers
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     view: article-grid
  #     columns: 2

  # 受賞歴
  - block: resume-awards
    id: awards
    content:
      title: Awards
      username: admin
    design:
      spacing:
        padding: [10, 0, 0, 0]

  # - block: collection
  #   id: awards
  #   content:
  #     title: Awards
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: post
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: date-title-summary
  #     # Reduce spacing
  #     spacing:
  #       padding: [10, 0, 0, 0]


  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: ""
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: false
  #   design:
  #     css_class: "bg-gray-100"
  #     view: citation
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     view: article-grid
  #     columns: 1
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!
        
        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
