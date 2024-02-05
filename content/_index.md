---
# Leave the homepage title empty to use the site title
title: 'Charalampos Lazaris'
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
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '1'
  - block: experience
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
        - title: Expert II, Oncology Data Science
          company: Novartis
          company_url: 'http://www.novartis.com'
          company_logo: org-novartis
          location: Cambridge, MA
          date_start: '2022-05-23'
          date_end: ''
          description: |2-
              Responsibilities include:
              * Analysing and integrating epigenomics data to uncover transcriptional dependencies in cancer.
        - title: Associated Scientist, Klarman Cell Observatory
          company: Broad Institute of MIT and Harvard
          company_url: 'https://www.broadinstitute.org'
          company_logo: org-bi
          location: Cambridge, MA
          date_start: '2020-06-01'
          date_end: '2022-05-22'
          description: Developed bioinformatics workflows, analysed NGS data, and completed postdoctoral work on transcriptional addiction in multiple myeloma. 
        - title: Bioinformatics Scientist
          company: Whitehead Institute
          company_url: 'https://wi.mit.edu'
          company_logo: org-wi
          location: Cambridge, MA
          date_start: '2020-01-27'
          date_end: '2022-05-22'
          description: Developed bioinformatics workflows, analysed NGS data, and completed postdoctoral work on transcriptional addiction in multiple myeloma.
        - title: Research Associate I
          company: University of California, San Diego
          company_url: 'https://www.ucsd.edu'
          company_logo: org-ucsd
          location: La Jolla, CA
          date_start: '2013-01-30'
          date_end: '2013-07-06'
          description: Investigated transcriptional response to aging in baker's yeast.
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.datacamp.com/completed/statement-of-accomplishment/track/7f8dd447aeda1e074be504b437729e7c5e4ded7d
          date_end: ''
          date_start: '2023-11-11'
          description: ''
          icon: datacamp
          organization: DataCamp
          organization_url: https://www.datacamp.com
          title: 'Julia Fundamentals'
          url: ''
        - certificate_url: https://www.coursera.org/account/accomplishments/verify/AU6AHPB7TW42
          date_end: '2022-03-20'
          date_start: '2022-03-20'
          description: ''
          icon: coursera
          organization: Coursera
          organization_url: https://www.coursera.org
          title: 'Julia Scientific Programming'
          url: ''
        - certificate_url: https://www.datacamp.com/completed/statement-of-accomplishment/track/8b7f4c4fddc05a37643e131139ffc5762027c7ab
          date_end: ''
          date_start: '2020-12-02'
          description: ''
          icon: datacamp
          organization: DataCamp
          organization_url: https://www.datacamp.com
          title: 'Python Developer'
          url: ''
        - certificate_url: https://www.datacamp.com/completed/statement-of-accomplishment/track/8b7f4c4fddc05a37643e131139ffc5762027c7ab
          date_end: ''
          date_start: '2020-11-28'
          description: ''
          icon: datacamp
          organization: DataCamp
          organization_url: https://www.datacamp.com
          title: 'SQL Server Developer'
          url: ''
        - certificate_url: https://www.coursera.org/account/accomplishments/verify/YYSE5KQ9XV
          date_end: '2014-07-08'
          date_start: '2014-07-08'
          description: ''
          icon: coursera
          organization: Coursera
          organization_url: https://www.datacamp.com
          title: 'R Programming'
          url: 'https://www.coursera.org/learn/r-programming'
        
    design:
      columns: '2'
 # - block: portfolio
 #   id: projects
 #   content:
 #     title: Projects
 #     filters:
 #       folders:
 #         - project
 #     # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
 #     default_button_index: 0
 #     # Filter toolbar (optional).
 #     # Add or remove as many filters (`filter_button` instances) as you like.
 #     # To show all items, set `tag` to "*".
 #     # To filter by a specific tag, set `tag` to an existing tag name.
 #     # To remove the toolbar, delete the entire `filter_button` block.
 #     buttons:
 #       - name: All
 #         tag: '*'
 #       - name: Deep Learning
 #         tag: Deep Learning
 #       - name: Other
 #         tag: Demo
 #   design:
 #     # Choose how many columns the section has. Valid values: '1' or '2'.
 #     columns: '1'
 #     view: showcase
 #     # For Showcase view, flip alternate rows?
 #     flip_alt_rows: false
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
      title: Publications
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
# - block: collection
#    id: posts
#    content:
#      title: Recent Posts
#      subtitle: ''
#      text: ''
#      # Choose how many pages you would like to display (0 = all pages)
#      count: 5
#      # Filter on criteria
#      filters:
#        folders:
#          - post
#        author: ""
#        category: ""
#        tag: ""
#        exclude_featured: false
#        exclude_future: false
#        exclude_past: false
#        publication_type: ""
#      # Choose how many pages you would like to offset by
#      offset: 0
#      # Page order: descending (desc) or ascending (asc) date.
#      order: desc
#    design:
#      # Choose a layout view
#      view: compact
#      columns: '2'
 # - block: tag_cloud
 #   content:
 #     title: Popular Topics
 #   design:
 #     columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      # email: lazaris@nyu.edu
      appointment_url: 'https://tidycal.com/lazaris'
      address:
        street: 250 Massachusetts Ave
        city: Cambridge
        region: MA
        postcode: '02139'
        country: United States
        country_code: US
      directions: Enter Building and take the stairs to Office on Floor 3
      office_hours:
        - 'Monday to Friday 9:00 to 17:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '42.36185'
        longitude: '-71.097557'  
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/chlazaris'
        # - icon: skype
        #  icon_pack: fab
        #  name: Skype Me
        #  link: 'skype:harris.lazaris17'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://nyu.zoom.us/j/5088350579'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      # form:
      #  provider: netlify
      #  formspree:
      #    id:
      #  netlify:
      #    # Enable CAPTCHA challenge to reduce spam?
      #    captcha: false
    design:
      columns: '2'
---
