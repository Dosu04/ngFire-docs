1. Import Angular Fire Auth Module to your app.module.ts file
``` 
import { AngularFireAuthModule } from '@angular/fire/compat/auth';


@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    AngularFireAuthModule,
  ],
  providers: [
  ],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

2. Create the view
``` 
<router-outlet></router-outlet>

<ng-container *ngIf="user$ | async as user">
  <ng-container *ngIf="user.user !== null; else NotSignedIn">
    <button (click)="onSignOutClick()">Sign Out</button>
    <h2>Welcome, {{ user.user.displayName }}!</h2>
    <p>email: {{ user.user.email }}!</p>
    <p>user id: {{ user.user.uid }}!</p>
    <img src="{{ user.user.photoURL }}" alt="" />
  </ng-container>
  <ng-template #NotSignedIn>
    <button (click)="onSignInClick()">Sign In with Google</button>
  </ng-template>
</ng-container>
```
