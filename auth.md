``` import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppRoutingModule } from './app-routing.module';
import { AppComponent } from './app.component';
// import { initializeApp, provideFirebaseApp } from '@angular/fire/app';
// import { provideAnalytics, getAnalytics, ScreenTrackingService, UserTrackingService } from '@angular/fire/analytics';
// import { provideAuth, getAuth } from '@angular/fire/auth';
// import { provideDatabase, getDatabase } from '@angular/fire/database';
// import { provideFirestore, getFirestore } from '@angular/fire/firestore';
// import { provideFunctions, getFunctions } from '@angular/fire/functions';
// import { provideMessaging, getMessaging } from '@angular/fire/messaging';
// import { providePerformance, getPerformance } from '@angular/fire/performance';
// import { provideRemoteConfig, getRemoteConfig } from '@angular/fire/remote-config';
// import { provideStorage, getStorage } from '@angular/fire/storage';
import { environment } from '../environments/environment';
import { AngularFireModule } from '@angular/fire/compat';
import { AngularFireAuthModule } from '@angular/fire/compat/auth';


@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule,
    AngularFireModule.initializeApp(environment.firebase),
    AngularFireAuthModule,
    // provideFirebaseApp(() => initializeApp(environment.firebase)),
    // provideAnalytics(() => getAnalytics()),
    // provideAuth(() => getAuth()),
    // provideDatabase(() => getDatabase()),
    // provideFirestore(() => getFirestore()),
    // provideFunctions(() => getFunctions()),
    // provideMessaging(() => getMessaging()),
    // providePerformance(() => getPerformance()),
    // provideRemoteConfig(() => getRemoteConfig()),
    // provideStorage(() => getStorage())
  ],
  providers: [
    // ScreenTrackingService, UserTrackingService
  ],
  bootstrap: [AppComponent]
})
export class AppModule { }