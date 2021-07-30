




## SCAFFOLD: 'NEW' LEADS 
This is an outline of what we currently have in place.
```html  
<div fxLayout="column" class="header-container">
  <antera-lib-kanban-header-grid></antera-lib-kanban-header-grid>
  <mat-drawer-container>
    <mat-drawer #drawer>
      <antera-lib-kanban-search></antera-lib-kanban-search>
    </mat-drawer>
    <mat-drawer-content>
      <div class="kanban-filter-bar-current">
        <antera-software-kanban-filter-bar></antera-software-kanban-filter-bar>
      </div>
      <div class="kanban-filter-quick-sticky">
        <anterasoftware-kanban-saved-search-bar></anterasoftware-kanban-saved-search-bar>
      </div>
      <div class="kanban-view-whole-container"></div>
      <ng-template #displayListView>
        <div *ngIf="leadsTableList?.length > 0">
          <div class="kanban-actions-bar">
            <anterasoftware-kanban-actions-bar></anterasoftware-kanban-actions-bar>
          </div>
          <div [ngClass]="">
            <anterasoftware-kanban-leads-list-view></anterasoftware-kanban-leads-list-view>
          </div>
        </div>
      </ng-template>
    </mat-drawer-content>
  </mat-drawer-container>
</div>
<div class="loading">
  <mat-spinner></mat-spinner>
</div>  
```  