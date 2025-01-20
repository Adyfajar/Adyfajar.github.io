---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.png
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: ' My Research'
      subtitle: ''
      text: |-
        I am actively involved in the development of new innovations, Here are some of my main focuses:

        - Developing Python learning modules that have been registered in Haki
        - Currently I am creating a business Application development to support the export of domestic umkm     products 
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 1
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: news
    content:
      title: News
      subtitle: ''
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
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      # Display name
      title: adi fajar saputra
      # Full name (for SEO)
      first_name: adi fajar
      last_name: saputra
      # Is this the primary user of the site?
      superuser: true
      # Highlight the author in author lists? (true/false)
      highlight_name: true
      # Role/position/tagline
      role: Software Engineering Student | Digital Creator
      # Organizations/Affiliations to display in Biography blox
      # Social network links
      # Need to use another icon? Simply download the SVG icon to your `assets/media/icons/` folder.
      profiles:
        - icon: at-symbol
          url: 'adyfajar.a.f.s@gmail.com'
          label: E-mail Me
        - icon: brands/instagram
          url: https://www.instagram.com/dyf_99/
        - icon: brands/github
          url: https://github.com/adyfajar
        - icon: brands/linkedin
          url: https://www.linkedin.com/adi-fajar-saputra
      spacing:
        padding: [0, 0, 0, 0]
      
---
