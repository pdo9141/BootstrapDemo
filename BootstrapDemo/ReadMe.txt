01) Bootstrap 3 takes mobile first philosophy (0-480, 480-768, 768-992, 992-1200, 1200 >)
02) .col-lg-xx: >= 1200px (desktop)
	.col-md-xx: >= 992px (landscape tablet)
	.col-sm-xx: >= 768px (portrait table)
	.col-xs-xx: < 768px (phone)
03) Mobile first means the devices that are least capable of rendering and processing HTML, CSS, JS will pull down the least resources
04) Major change from Bootstrap 2, breaks existing clients
05) Grid system is 12, not required but should be
06) Go to bootswatch.com, pick a theme you like, create new theme css file, reference it after bootstrap.min.css
07) Use img-responsive to scale nicely to parent element
08) Use .btn .btn-primary .btn-success .btn-warning .btn-muted .btn-lg .btn-sm, etc. for buttons or hyperlinks
09) Use wspan and class glyphicon to display icons
10) Use .navbar .navbar-default . navbar-header .nav .navbar-nav .navbar-right .active for navigation menu
11) Use .navbar-collapse .collapse .navbar-toggle and data-toggle="collapse" data-target=".navbar-collapse" to navigation collapse
12) To force the menu to always show, use .navbar-fixed-top, make sure you add a bit of CSS to adjust body (body { margin-top: 70px; })
13) Use .list-unstyled to remove bullet from list, use .list-inline to force horizontal left to right for list
14) Use .list-group and .list-group-item for IOs like table experience
15) Use .active for list as well
16) Add <span class="badge">15</span> to list for comments, read, unread, etc. You can also use <span class="badge"><span class="glyphicon glyphicon-earphone"></span></span>                        
17) Wrap table around div.row and div.col-md-6 to force table to be half the container
18) Use .table-responsive on a parent div (don't put this class on table itself, will have no effect) to add scrollbars for the table in mobile view
19) Use .form-group .form-control for form elements, you can use .btn .btn-success on submit buttons as well (on smaller devices it'll go into .form-horizontal)
20) Use .form-horizontal .control-label for horizontal forms
21) 




Bootstrap Components