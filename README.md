# Some_Angular_Issues:

## Routing:
1) Scroll to top on navigation in Angular:

    In Angular applications using the default routing settings, the scroll position remains unchanged when moving between pages. This means that if you scroll down on one page and click a link to navigate, the next page will open with the scroll position retained.
   <br>
    To solve that, you can use the "scrollPositionRestoration" option and set it to "enabled".

        @NgModule({
        imports: [
        RouterModule.forRoot(routes, { scrollPositionRestoration: "enabled" }),
        ],
        exports: [RouterModule],
        })
        export class AppRoutingModule {}
