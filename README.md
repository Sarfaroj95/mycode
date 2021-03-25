> Angular Some Setup
- AppModule
- HttpCmodule
- FormModule
- RouterModule

### AppModule
```
import { HttpClientModule } from "@angular/common/http";
import { AuthService } from "./share/service.service";
	
 imports: [
    HttpClientModule
],
providers: [AuthService],
```
>before use HttpClient & Service

### Service

```
import { Injectable } from "@angular/core"; 
import { HttpClient } from "@angular/common/http"; 
import { Observable } from "rxjs";

@Injectable({
  providedIn: "root"
})

export class AuthService { 

 private baseurl = environment.url; 
 private OptionWhatisForUrl = this.baseurl + "whatisfor/";

 public getData(): Observable<any[]> {
    return this.http.get<any[]>(this.OptionWhatisForUrl);
  }
}
```

### FormModule

```
import { FormsModule, ReactiveFormsModule } from "@angular/forms";

 imports: [
    FormsModule,
    ReactiveFormsModule,
  ],
```

>Before Reactive FormModule

####  Used tc File
```
import { FormBuilder, FormGroup, Validators } from "@angular/forms";

 loginForm: FormGroup;

 constructor(private fb: FormBuilder) { }


 initForm() {
    this.steponeForm = this.fb.group({
      money: ["", [Validators.required,Validators.pattern("^[1-9][0-9,]+$"),Validators.maxLength(12)]],
})

```
###### Validator regex
> "^[a-zA-Z ]*$" For name
> "^[1-9][0-9,]+$" For Number
> "^[a-zA-Z0-9.!#$%&’*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:.[a-zA-Z0-9-]+)*$" For Email ID

###### Inside Html
> [formGroup]="steponeForm" (ngSubmit)="onSubmit()"

## Router System
###### AppModule

```
import { AppRoutingModule } from './app-routing.module';

 imports: [
    AppRoutingModule,
  ],
```
> When use router must be import router module in AppModule

###### Router Moudle
```
import { NgModule } from '@angular/core';
import { RouterModule, Routes } from '@angular/router';
import { ChartsComponent } from './components/charts/charts.component';


const routes: Routes = [
  { path: '', component: DataGridComponent },
  { path: 'charts', component: ChartsComponent }
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }
```
