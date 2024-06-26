---
displayed_sidebar: wordpress-plugin
---

# Publish

## Publish Entity

When saved, entities are created as `custom posts` in the local WordPress installation and are accessible from the [WordLift vocabulary](/pages/key-concepts#vocabulary).

:::info Note
The URL for an entity page is as follows::

[http://](#)<*name-of-your-wordpress-site*>/?entity=<*name-of-the–entity*>
:::

### Metadata being added to Entity pages

### RDF representation of the Entity

By clicking on the **View Linked Data** button (right after the *Permalink* in the editor) the **RDF representation of the entity** is displayed using [LodView](http://lodview.it/).

![image](./images/wordlift-publish-entity-view-linked-data.png)

![image](./images/wordlift-publish-entity-lodview.png)

In this example you can see the relation being created between the entity *\[Mars\]* and the entity *\[Solar System\]* (`dcterms:relation`). This relation has been created from the [entity page](/pages/edit-entity#linking-other-entities) page by annotating the description of the entity.

![image](./images/wordlift-publish-entity-lodlive.png)

You can also see (in this last image using [LodLive](http://lodlive.it/)) the `sameAs` attributes.

## Publish Post/Page

Posts and Pages with **WordLift** are annotated using the `schema.org` vocabulary.
The *schema markup* is a code (a semantic vocabulary) to help search engines return more informative results for their users.

### Metadata being added to Post/Page

By clicking on the **Test Google Rich Snippets** button (right after the *Permalink* in the editor) you can see the list of entities being added to the content from the **Google Structured Data Testing Tool**.

![image](./images/wordlift-publish-post-test-structured-data.png)

![image](./images/wordlift-publish-structured-data-testing.png)

In this example we're telling search engines that this post could be relevant for searches related to the *\[Solar System\]*.

### RDF representation of the Post/Page

By clicking on the **View Linked Data** button (right after the *Permalink* in the editor) the **RDF representation of the post** is displayed using [LodView](http://lodview.it/).

As of today, the data being represented in RDF for each post or page include:

- schema-org:**datePublished**
- schema-org:**dateModified**
- schema-org:**interactionCount**
- rdfs:**label**
- rdf:**type**
- schema-org:**url**
- dcterms:**references**
- schema-org:**author**

![image](./images/wordlift-publish-post-lodview.png)

:::info Note
In the RDF representation of the posts you can find all entities related to a post (or a page) by looking at the `dcterms:references` attribute
:::

The attributes describing the posts can be browsed. In this example by clicking on the entity *\[Solar System\]* you will be able (directly from [LodView](http://lodview.it/)) to consult and read the data publish on that entity by **WordLift**.

You can now continue to the [Discover](/pages/discover) page.
