# tabs-hartford
dynamic tab load component

# Html
<div class="container ">
    <div class="row">
      <div class="col-12">
        <div class="card">
          <div class="card-body">
            <ul class="nav nav-tabs">
                <li *ngFor="let key of keys">
                    <a data-toggle="tab" href="{{'#'+key}}">{{key}}</a>
                </li>
              </ul>
            
              <div class="tab-content">
                    <div id="1" class="tab-pane fade">
                        <h3>Home</h3>
                    </div>
                    <div id="2" class="tab-pane fade">
                        <h3>Party</h3>
                    </div>
                    <div id="3" class="tab-pane fade">
                        <h3>Auto</h3>
                    </div>
              </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  
  # Ts
  
 import { Component, OnInit } from '@angular/core';

@Component({
  selector: 'app-tabs',
  templateUrl: './tabs.component.html',
  styleUrls: ['./tabs.component.css']
})
export class TabsComponent implements OnInit {
  keys:String[]
  constructor() {
    this.keys=['1','2','3']
   }

  ngOnInit(): void {
  }

}

# Bootstrap links

  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
