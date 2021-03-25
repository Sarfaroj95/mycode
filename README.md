- AppModule
- HttpClient

### `AppModule`
import { HttpClientModule } from "@angular/common/http";
 
before use HttpClient

### `Service`
> Service
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