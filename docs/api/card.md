---
title: "ion-card"
hide_table_of_contents: true
demoUrl: "/docs/demos/api/card/index.html"
demoSourceUrl: "https://github.com/ionic-team/ionic-docs/tree/main/static/demos/api/card/index.html"
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';
import TOCInline from '@theme/TOCInline';

import Props from '@site/static/auto-generated/card/props.md';
import Events from '@site/static/auto-generated/card/events.md';
import Methods from '@site/static/auto-generated/card/methods.md';
import Parts from '@site/static/auto-generated/card/parts.md';
import CustomProps from '@site/static/auto-generated/card/custom-props.md';
import Slots from '@site/static/auto-generated/card/slots.md';

import EncapsulationPill from '@components/page/api/EncapsulationPill';

<head>
  <title>ion-card: Card UI Components for Ionic Framework API</title>
  <meta name="description" content="ion-card UI components are entry points to more detailed information. Cards can be single components or made up of some header, title, subtitle, and content." />
</head>

<EncapsulationPill type="shadow" />

<h2 className="table-of-contents__title">Contents</h2>

<TOCInline
  toc={toc}
  maxHeadingLevel={2}
/>



Cards are a standard piece of UI that serves as an entry point to more detailed
information. A card can be a single component, but is often made up of some
header, title, subtitle, and content. `ion-card` is broken up into several
sub-components to reflect this. Please see `ion-card-content`,
`ion-card-header`, `ion-card-title`, `ion-card-subtitle`.



## Usage

<Tabs groupId="framework" defaultValue="angular" values={[{ value: 'angular', label: 'Angular' }, { value: 'javascript', label: 'Javascript' }, { value: 'react', label: 'React' }, { value: 'stencil', label: 'Stencil' }, { value: 'vue', label: 'Vue' }]}>

<TabItem value="angular">

```html
<ion-card>
  <ion-card-header>
    <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
    <ion-card-title>Card Title</ion-card-title>
  </ion-card-header>

  <ion-card-content>
    Keep close to Nature's heart... and break clear away, once in awhile,
    and climb a mountain or spend a week in the woods. Wash your spirit clean.
  </ion-card-content>
</ion-card>

<ion-card>
  <ion-item>
    <ion-icon name="pin" slot="start"></ion-icon>
    <ion-label>ion-item in a card, icon left, button right</ion-label>
    <ion-button fill="outline" slot="end">View</ion-button>
  </ion-item>

  <ion-card-content>
    This is content, without any paragraph or header tags,
    within an ion-card-content element.
  </ion-card-content>
</ion-card>

<ion-card>
  <ion-item href="#" class="ion-activated">
    <ion-icon name="wifi" slot="start"></ion-icon>
    <ion-label>Card Link Item 1 activated</ion-label>
  </ion-item>

  <ion-item href="#">
    <ion-icon name="wine" slot="start"></ion-icon>
    <ion-label>Card Link Item 2</ion-label>
  </ion-item>

  <ion-item class="ion-activated">
    <ion-icon name="warning" slot="start"></ion-icon>
    <ion-label>Card Button Item 1 activated</ion-label>
  </ion-item>

  <ion-item>
    <ion-icon name="walk" slot="start"></ion-icon>
    <ion-label>Card Button Item 2</ion-label>
  </ion-item>
</ion-card>
```

</TabItem>


<TabItem value="javascript">

```html
<ion-card>
  <ion-card-header>
    <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
    <ion-card-title>Card Title</ion-card-title>
  </ion-card-header>

  <ion-card-content>
    Keep close to Nature's heart... and break clear away, once in awhile,
    and climb a mountain or spend a week in the woods. Wash your spirit clean.
  </ion-card-content>
</ion-card>

<ion-card>
  <ion-item>
    <ion-icon name="pin" slot="start"></ion-icon>
    <ion-label>ion-item in a card, icon left, button right</ion-label>
    <ion-button fill="outline" slot="end">View</ion-button>
  </ion-item>

  <ion-card-content>
    This is content, without any paragraph or header tags,
    within an ion-card-content element.
  </ion-card-content>
</ion-card>

<ion-card>
  <ion-item href="#" class="ion-activated">
    <ion-icon name="wifi" slot="start"></ion-icon>
    <ion-label>Card Link Item 1 activated</ion-label>
  </ion-item>

  <ion-item href="#">
    <ion-icon name="wine" slot="start"></ion-icon>
    <ion-label>Card Link Item 2</ion-label>
  </ion-item>

  <ion-item class="ion-activated">
    <ion-icon name="warning" slot="start"></ion-icon>
    <ion-label>Card Button Item 1 activated</ion-label>
  </ion-item>

  <ion-item>
    <ion-icon name="walk" slot="start"></ion-icon>
    <ion-label>Card Button Item 2</ion-label>
  </ion-item>
</ion-card>
```

</TabItem>


<TabItem value="react">

```tsx
import React from 'react';
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar, IonCard, IonCardHeader, IonCardSubtitle, IonCardTitle, IonCardContent, IonItem, IonIcon, IonLabel, IonButton } from '@ionic/react';
import { pin, wifi, wine, warning, walk } from 'ionicons/icons';

export const CardExamples: React.FC = () => {
  return (
    <IonPage>
      <IonHeader>
        <IonToolbar>
          <IonTitle>CardExamples</IonTitle>
        </IonToolbar>
      </IonHeader>
      <IonContent>
        <IonCard>
          <IonCardHeader>
            <IonCardSubtitle>Card Subtitle</IonCardSubtitle>
            <IonCardTitle>Card Title</IonCardTitle>
          </IonCardHeader>

          <IonCardContent>
            Keep close to Nature's heart... and break clear away, once in awhile,
            and climb a mountain or spend a week in the woods. Wash your spirit clean.
      </IonCardContent>
        </IonCard>

        <IonCard>
          <IonItem>
            <IonIcon icon={pin} slot="start" />
            <IonLabel>ion-item in a card, icon left, button right</IonLabel>
            <IonButton fill="outline" slot="end">View</IonButton>
          </IonItem>

          <IonCardContent>
            This is content, without any paragraph or header tags,
            within an ion-cardContent element.
      </IonCardContent>
        </IonCard>

        <IonCard>
          <IonItem href="#" className="ion-activated">
            <IonIcon icon={wifi} slot="start" />
            <IonLabel>Card Link Item 1 activated</IonLabel>
          </IonItem>

          <IonItem href="#">
            <IonIcon icon={wine} slot="start" />
            <IonLabel>Card Link Item 2</IonLabel>
          </IonItem>

          <IonItem className="ion-activated">
            <IonIcon icon={warning} slot="start" />
            <IonLabel>Card Button Item 1 activated</IonLabel>
          </IonItem>

          <IonItem>
            <IonIcon icon={walk} slot="start" />
            <IonLabel>Card Button Item 2</IonLabel>
          </IonItem>
        </IonCard>
      </IonContent>
    </IonPage>
  );
};

```

</TabItem>


<TabItem value="stencil">

```tsx
import { Component, h } from '@stencil/core';

@Component({
  tag: 'card-example',
  styleUrl: 'card-example.css'
})
export class CardExample {
  render() {
    return [
      <ion-card>
        <ion-card-header>
          <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
          <ion-card-title>Card Title</ion-card-title>
        </ion-card-header>

        <ion-card-content>
          Keep close to Nature's heart... and break clear away, once in awhile,
          and climb a mountain or spend a week in the woods. Wash your spirit clean.
        </ion-card-content>
      </ion-card>,

      <ion-card>
        <ion-item>
          <ion-icon name="pin" slot="start"></ion-icon>
          <ion-label>ion-item in a card, icon left, button right</ion-label>
          <ion-button fill="outline" slot="end">View</ion-button>
        </ion-item>

        <ion-card-content>
          This is content, without any paragraph or header tags,
          within an ion-card-content element.
        </ion-card-content>
      </ion-card>,

      <ion-card>
        <ion-item href="#" class="ion-activated">
          <ion-icon name="wifi" slot="start"></ion-icon>
          <ion-label>Card Link Item 1 activated</ion-label>
        </ion-item>

        <ion-item href="#">
          <ion-icon name="wine" slot="start"></ion-icon>
          <ion-label>Card Link Item 2</ion-label>
        </ion-item>

        <ion-item class="ion-activated">
          <ion-icon name="warning" slot="start"></ion-icon>
          <ion-label>Card Button Item 1 activated</ion-label>
        </ion-item>

        <ion-item>
          <ion-icon name="walk" slot="start"></ion-icon>
          <ion-label>Card Button Item 2</ion-label>
        </ion-item>
      </ion-card>
    ];
  }
}
```

</TabItem>


<TabItem value="vue">

```html
<template>
  <ion-card>
    <ion-card-header>
      <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
      <ion-card-title>Card Title</ion-card-title>
    </ion-card-header>

    <ion-card-content>
      Keep close to Nature's heart... and break clear away, once in awhile,
      and climb a mountain or spend a week in the woods. Wash your spirit clean.
    </ion-card-content>
  </ion-card>

  <ion-card>
    <ion-item>
      <ion-icon :icon="pin" slot="start"></ion-icon>
      <ion-label>ion-item in a card, icon left, button right</ion-label>
      <ion-button fill="outline" slot="end">View</ion-button>
    </ion-item>

    <ion-card-content>
      This is content, without any paragraph or header tags,
      within an ion-card-content element.
    </ion-card-content>
  </ion-card>

  <ion-card>
    <ion-item href="#" class="ion-activated">
      <ion-icon :icon="wifi" slot="start"></ion-icon>
      <ion-label>Card Link Item 1 activated</ion-label>
    </ion-item>

    <ion-item href="#">
      <ion-icon :icon="wine" slot="start"></ion-icon>
      <ion-label>Card Link Item 2</ion-label>
    </ion-item>

    <ion-item class="ion-activated">
      <ion-icon :icon="warning" slot="start"></ion-icon>
      <ion-label>Card Button Item 1 activated</ion-label>
    </ion-item>

    <ion-item>
      <ion-icon :icon="walk" slot="start"></ion-icon>
      <ion-label>Card Button Item 2</ion-label>
    </ion-item>
  </ion-card>
</template>

<script>
import { IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle, IonIcon, IonItem, IonLabel } from '@ionic/vue';
import { pin, walk, warning, wifi, wine } from 'ionicons/icons';
import { defineComponent } from 'vue';

export default defineComponent({
  components: { IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle, IonIcon, IonItem, IonLabel }
  setup() {
    return { warning };
  }
});
</script>
```

</TabItem>

</Tabs>

## Properties
<Props />

## Events
<Events />

## Methods
<Methods />

## CSS Shadow Parts
<Parts />

## CSS Custom Properties
<CustomProps />

## Slots
<Slots />