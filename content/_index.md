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
