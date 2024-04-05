---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: skills
    id: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '1'
  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: PhD in Mechanical Engineering
          company: Northwestern Polytechnical University
          company_url: ''
          #company_logo: org-gc
          company_logo: NWPU
          location: Xi'an
          date_start: '2021-03-01'
          date_end: ''
          description: |2-
              Dissertation proposal:
              * Research on the equipment and experiments of metal droplet 3D printing based on coaxial shielding gas supply.
        - title: MRes in Mechanical Engineering
          company: Northwestern Polytechnical University
          company_url: ''
          company_logo: NWPU
          location: Xi'an
          date_start: '2018-09-01'
          date_end: '2021-03-01'
          description: |2-
              Graduation project:
              * Micro-domain protection of tin alloy bump printing and its experimental research.

        - title: BEng in Industrial Design
          company: Northwestern Polytechnical University
          company_url: ''
          company_logo: NWPU
          location: Xi'an
          date_start: '2014-09-01'
          date_end: '2018-07-01'
          description: |2-
              Graduation project:
              * Appearance and human-machine interface design for three-dimensional microcircuit printing equipment.
    design:
      columns: '2'
  - block: accomplishments
    id: awards
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      #title: 'Accomplish&shy;ments'
      title: 'Awards'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - #certificate_url: https://www.coursera.org
          date_end: ''
          date_start: '2021-03-01'
          description: 'in 2021, and 2018'
          icon: NWPU
          organization: Northwestern Polytechnical University
          organization_url:  https://www.nwpu.edu.cn/
          title: First-Class Academic Scholarship
          url: ''
        - #certificate_url: https://www.datacamp.com
          date_end: ''
          date_start: '2018-03-01'
          description: ''
          icon: NWPU
          organization: Northwestern Polytechnical University
          organization_url: https://www.nwpu.edu.cn/
          title: 'Recommended exemption qualifications for masters'
          url: ''
        - #certificate_url: https://www.edx.org
          date_end: ''
          date_start: '2017-08-01'
          description: The 6th National Ocean Vehicle Design and fabrication Competition.
          icon: CSIC
          organization:  China Shipbuilding Industry Group Co., Ltd
          organization_url: http://www.csic.com.cn/
          title: National Special Prize
          url: ''
    design:
      columns: '2'
  # - block: collection
  #   id: posts
  #   content:
  #     title: Recent Posts
  #     subtitle: ''
  #     text: ''
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       folders:
  #         - post
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
  #     view: compact
  #     columns: '2'
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
        - name: Main In-charge
          tag: Main In-charge
        - name: Main Participant
          tag: Main Participant
#          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    id: gallery
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
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
        exclude_featured: false
    design:
      columns: '2'
      view: citation
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     columns: '2'
  #     view: compact

  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
  - block: contact
    id: contact
    content:
    title: Contact
    subtitle: null
    text: "Good communication is the beginning of learning and progress, welcome to contact me!"
    iframe_code: |
      <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSde3zVBxbc9EXWUtxL_hAzcvpQTyvxfIWoClqwyN1bzuJxVpA/viewform?embedded=true" width="640" height="684" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
    design:
    columns: '2'

---
