### `AppModule`
import { HttpClientModule } from "@angular/common/http";
 
before use HttpClient

### `Service`
import { Injectable } from "@angular/core"; <br/>
import { HttpClient } from "@angular/common/http";
import { Observable } from "rxjs";

@Injectable({
  providedIn: "root"
})



export class AuthService { 

 private baseurl = environment.url; <br/>
 private OptionWhatisForUrl = this.baseurl + "whatisfor/";

 public getData(): Observable<any[]> {
    return this.http.get<any[]>(this.OptionWhatisForUrl);
  }


}