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
21) Use .btn-group to treat many buttons as one singular display. Use .btn-group-vertical to go vertical, use .btn-group-sm to change size
22) Use data-toggle="buttons" and change button types to labels and then add input checkbox to create toggleable buttons, you can use radio buttons as well
23) Use .dropdown, data-toggle="dropdown", .dropdown-menu, .divider, .disabled, .active for dropdown
24) If you want a button group item to display a dropdown, change .dropdown to .btn-group
25) Use .input-group and .input-group-addon to add information indicator to inputs, you can add before or after or both, you can use glyphicons as well
26) Use .pager, .pagination, .pagination-sm, .disabled, .active, .previous, .next for paging
27) Use .thumbnail and .caption for thumbnails
28) Use .panel, .panel-default, .panel-primary, .panel-info, .panel-title, .panel-footer, .panel-body to get panel semantics, styling, spacing, etc.
29) Use .well, .well-sm, .well-lg for panel-like sections 
30) Use data-toggle="collapse" and class="collapse" for collapse functionality, use class collapse in to show section initially
31) To build accordian, use .panel-group, .panel-collapse, .collapse
32) For modals, use .modal, .fade, .modal-dialog, .modal-content, data-dismiss="modal", data-toggle="modal"
33) You can hook into Bootstrap custom events in JS, e.g., 
	$sentDialog.on("hidden.bs.modal", function () {
        alert("close");
    });
34) For tabs use .active, .tab-pane .tab-content, data-toggle="tab", .nav-justified, 
35) For tooltips use data-toggle="tooltip", title="Press Here", data-placement="right", data-delay="500", data-html="true"
	$("#contactForm input[type=submit]").tooltip();
	$("#contactForm input[type=submit]").tooltip({
        placement: "left"        
    });
36) For alerts use .alert, .alert-warning, .collapse, data-dismiss="alert" and script it to not remove from DOM since we used data-dismiss="alert"
	$sentAlert.on("close.bs.alert", function () {
        $sentAlert.hide();
        return false;
    });
37) For carousel use .carousel, .slide, .carousel-indicators, data-interval="2000", .active, data-slide-to="0", .carousel-inner, .item
	$("#theCarousel").carousel();
38) For carousel navigation and caption use .carousel-control, .left, .right, data-slide="prev", data-slide="next", <span class="icon-prev"></span>, carousel-caption