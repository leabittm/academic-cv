---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biographie
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    content:
      title: Autres textes
      text: 
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: citation
  - block: portfolio
    id: teaching
    content:
      title: Enseignement
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
#      buttons:
#        - name: All
#          tag: '*'
#        - name: Deep Learning
#          tag: Deep Learning
#        - name: Other
#          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: compact
#      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: accomplishments
    id: other_activities
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: Autres activités
#      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - date_start: '2024-09-01'
          date_end: ''
          description: ''
          organization: Université de Strasbourg
          title: Organisatrice du [**Séminaire ART**](https://irma.math.unistra.fr/seminaires/seminaire-art.html)
#          url: ''
        - date_end: '2023-01-06'
          date_start: '2021-09-01'
          description: ''
          organization: University of Edinburgh
          title: Organisatrice du [**Hodge Seminar**](https://sites.google.com/view/hodge-seminars/), puis du [**Algebra Seminar**](https://sites.google.com/view/hodge-seminars/)
#          url: ''
        - date_end: '2023-01-06'
          date_start: '2021-09-01'
          description: ''
          organization: University of Edinburgh
          title: Réprésentante des postdocs auprès du [*Equality, Diversity and Inclusion* committee](https://www.maths.ed.ac.uk/school-of-mathematics/about-us/equality-diversity-and-inclusion)
#          url: 'https://www.maths.ed.ac.uk/school-of-mathematics/about-us/equality-diversity-and-inclusion'
        - date_end: '2019-08-31'
          date_start: '2017-09-01'
          description: ''
          organization: Université Paris Diderot
          title: Organisatrice des *Rencontres Master-Doctorants*
          description : Rencontres biannuelles entre etudiants de master et doctorants
#          url: 'https://www.maths.ed.ac.uk/school-of-mathematics/about-us/equality-diversity-and-inclusion'
        - date_end: '2019-08-31'
          date_start: '2017-09-01'
          description: ''
          organization: Université Paris Diderot
          title: Membre du [*Comité Parité*](https://www.imj-prg.fr/comite-parite/)
#          url: 'https://www.imj-prg.fr/comite-parite/'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: 
      # Contact (add or remove contact options as necessary)
      email: lea.bittmann@math.unistra.fr
      #phone: 888 888 88 88
      #appointment_url: 'https://calendly.com'
      address:
        street: IRMA, Université de Strasbourg, 7 rue René Descartes
        city: Strasbourg
        #region: CA
        postcode: '67000'
        country: France
        #country_code: FR
      directions: Bureau 218
      #office_hours:
      #  - 'Monday 10:00 to 13:00'
      #  - 'Wednesday 09:00 to 10:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      #coordinates:
      #  latitude: '37.4275'
      #  longitude: '-122.1697'  
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      #form:
      #  provider: netlify
      #  formspree:
      #    id:
      #  netlify:
          # Enable CAPTCHA challenge to reduce spam?
      #    captcha: false
    design:
      columns: '2'
---
