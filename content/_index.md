---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: why 
  - block: features
    content:
      title: Skills
      items:
        - name: C; C++; Python; Taichi
          # description: 90%
          # icon: r-project
          # icon_pack: fab
        - name: Vulkan; DirectX; OpenGL
          # description: 100%
          # icon: chart-line
          # icon_pack: fas
        - name: Blender; Houdini; ZENO
          # description: 10%
          # icon: camera-retro
          # icon_pack: fas
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Rendering 
          tag: Rendering
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: featured
    content:
      title: Selected Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: experience
    content:
      title: Experience
      # Date format for experience
      # date_format: July 2024
      # # Experiences.
      # #   Add/remove as many `experience` items below as you like.
      # #   Required fields are `title`, `company`, and `date_start`.
      # #   Leave `date_end` empty if it's your current employer.
      # #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      # items:
      #   - title: Intern
      #     company: ZenusTech
      #     company_url: ''
      #     company_logo: org-gc
      #     location: Shenzhen
      #     date_start: '2024-07-01'
      #     date_end: '2024-09-01'
      #     description: |2-
      #         Responsibilities include:
      #         * Researching
      #   - title: 
      #     company: 
      #     company_url: ''
      #     company_logo: org-x
      #     location: 
      #     date_start: ''
      #     date_end: ''
      #     description: Taught electronic engineering and researched semiconductor physics.
    design:
      columns: '2'
  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
  # - block: markdown
  #   content:
  #     title: Art 
  #     subtitle: ''
  #     text: |-
  #       {{< gallery album="demo" >}}
  #   design:
  #     columns: '1'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Feel free to contact me. 
      # Contact (add or remove contact options as necessary)
      email: nn9.yang@gmail.com
      phone: +86 13226008326
      # appointment_url: 'https://calendly.com'
      address:
        # street: None
        city: Zhuhai
        region: GuangDong
        postcode: '519000'
        country: China
        country_code: CN
      # directions: None
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      contact_links:
        # - icon: skype
        #   icon_pack: fab
        #   name: Skype Me
        #   link: 'skype:echo123?call'
        # - icon: video
        #   icon_pack: fas
        #   name: Zoom Me
        #   link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
