```tsx
import React from 'react';
import { IonLabel, IonHeader, IonSegment, IonSegmentButton, IonToolbar } from '@ionic/react';

function Example() {
  return (
    <IonHeader>
      <IonToolbar>
        <IonSegment value="all">
          <IonSegmentButton value="all">
            <IonLabel>All</IonLabel>
          </IonSegmentButton>
          <IonSegmentButton value="favorites">
            <IonLabel>Favorites</IonLabel>
          </IonSegmentButton>
        </IonSegment>
      </IonToolbar>
    </IonHeader>
  );
}
export default Example;
```
