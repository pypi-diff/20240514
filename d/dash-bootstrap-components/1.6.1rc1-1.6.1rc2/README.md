# Comparing `tmp/dash_bootstrap_components-1.6.1rc1.tar.gz` & `tmp/dash_bootstrap_components-1.6.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_bootstrap_components-1.6.1rc1.tar", last modified: Mon May  6 17:15:01 2024, max compression
+gzip compressed data, was "dash_bootstrap_components-1.6.1rc2.tar", last modified: Tue May 14 20:54:04 2024, max compression
```

## Comparing `dash_bootstrap_components-1.6.1rc1.tar` & `dash_bootstrap_components-1.6.1rc2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:15:01.300337 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Accordion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/AccordionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Breadcrumb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Button.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ButtonGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardFooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardImg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardImgOverlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardLink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Carousel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Checklist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Col.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Container.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/DropdownMenu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/DropdownMenuItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Fade.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormFeedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormFloating.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormText.py
--rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/InputGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/InputGroupText.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ListGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ListGroupItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalFooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Nav.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavLink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Navbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarBrand.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarSimple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarToggler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Offcanvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Popover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/PopoverBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/PopoverHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/RadioButton.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/RadioItems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Row.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Textarea.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   233998 2024-05-06 17:14:46.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   363181 2024-05-06 17:14:49.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/themes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-06 17:15:01.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-06 17:15:01.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:15:01.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 17:15:01.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 17:15:01.000000 dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/landing-page.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:15:01.316337 dash_bootstrap_components-1.6.1rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_components_as_props.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_navlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_popover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_positional_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 17:14:10.000000 dash_bootstrap_components-1.6.1rc1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:04.116970 dash_bootstrap_components-1.6.1rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-14 20:54:04.116970 dash_bootstrap_components-1.6.1rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:04.100970 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:04.112970 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Accordion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/AccordionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Breadcrumb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ButtonGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardFooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardImg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardImgOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardLink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Carousel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Checklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/DropdownMenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/DropdownMenuItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Fade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/FormFeedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/FormFloating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/FormText.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/InputGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/InputGroupText.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ListGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ListGroupItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ModalBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ModalFooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ModalHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ModalTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Nav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/NavItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/NavLink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Navbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/NavbarBrand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/NavbarSimple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/NavbarToggler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Offcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Popover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/PopoverBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/PopoverHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/RadioButton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/RadioItems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Textarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   234091 2024-05-14 20:53:48.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/dash_bootstrap_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   363671 2024-05-14 20:53:51.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:04.116970 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-14 20:54:04.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-14 20:54:04.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:54:04.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 20:54:04.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 20:54:04.000000 dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/landing-page.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-14 20:54:04.116970 dash_bootstrap_components-1.6.1rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:54:04.116970 dash_bootstrap_components-1.6.1rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/tests/test_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/tests/test_components_as_props.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/tests/test_navlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/tests/test_popover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/tests/test_positional_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/tests/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 20:53:10.000000 dash_bootstrap_components-1.6.1rc2/tests/test_version.py
```

### Comparing `dash_bootstrap_components-1.6.1rc1/LICENSE` & `dash_bootstrap_components-1.6.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/PKG-INFO` & `dash_bootstrap_components-1.6.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-bootstrap-components
-Version: 1.6.1rc1
+Version: 1.6.1rc2
 Summary: Bootstrap themed components for use in Plotly Dash
 Home-page: https://dash-bootstrap-components.opensource.faculty.ai/
 Author: Faculty
 Author-email: opensource@faculty.ai
 License: Apache Software License
 Project-URL: Bug Reports, https://github.com/facultyai/dash-bootstrap-components/issues
 Project-URL: Source, https://github.com/facultyai/dash-bootstrap-components/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.1rc1
+Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.1rc2
 Summary: Bootstrap themed components for use in Plotly Dash Home-page: https://
 dash-bootstrap-components.opensource.faculty.ai/ Author: Faculty Author-email:
 opensource@faculty.ai License: Apache Software License Project-URL: Bug
 Reports, https://github.com/facultyai/dash-bootstrap-components/issues Project-
 URL: Source, https://github.com/facultyai/dash-bootstrap-components/
 Classifier: Framework :: Dash Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `dash_bootstrap_components-1.6.1rc1/README.md` & `dash_bootstrap_components-1.6.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/__init__.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Accordion.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Accordion.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/AccordionItem.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/AccordionItem.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Alert.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Alert.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Badge.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Badge.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Breadcrumb.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Breadcrumb.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Button.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Button.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ButtonGroup.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ButtonGroup.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Card.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Card.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardBody.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardBody.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardFooter.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardFooter.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardGroup.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardGroup.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardHeader.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardHeader.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardImg.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardImg.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardImgOverlay.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardImgOverlay.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/CardLink.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/CardLink.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Carousel.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Carousel.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Checkbox.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Checkbox.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Checklist.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Checklist.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Col.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Col.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Collapse.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Collapse.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Container.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Container.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/DropdownMenu.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/DropdownMenu.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/DropdownMenuItem.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/DropdownMenuItem.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Fade.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Fade.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Form.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Form.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormFeedback.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/FormFeedback.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormFloating.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/FormFloating.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/FormText.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/FormText.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Input.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Input.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/InputGroup.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/InputGroup.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/InputGroupText.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/InputGroupText.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Label.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Label.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ListGroup.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ListGroup.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ListGroupItem.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ListGroupItem.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Modal.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Modal.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalBody.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ModalBody.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalFooter.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ModalFooter.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalHeader.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ModalHeader.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/ModalTitle.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/ModalTitle.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Nav.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Nav.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavItem.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/NavItem.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavLink.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/NavLink.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Navbar.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Navbar.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarBrand.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/NavbarBrand.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarSimple.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/NavbarSimple.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/NavbarToggler.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/NavbarToggler.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Offcanvas.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Offcanvas.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Pagination.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Pagination.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Placeholder.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Placeholder.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Popover.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Popover.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/PopoverBody.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/PopoverBody.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/PopoverHeader.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/PopoverHeader.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Progress.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Progress.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/RadioButton.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/RadioButton.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/RadioItems.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/RadioItems.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Row.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Row.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Select.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Select.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Spinner.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Spinner.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Stack.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Stack.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Switch.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Switch.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tab.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Tab.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Table.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tabs.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Tabs.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Textarea.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Textarea.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,18 +132,19 @@
 - n_clicks_timestamp (number; default -1):
     An integer that represents the time (in ms since 1970) at which
     n_clicks changed. This can be used to tell which button was
     changed most recently.
 
 - n_submit (number; default 0):
     Number of times the `Enter` key was pressed while the textarea had
-    focus.
+    focus. Only updates if submit_on_enter is True.
 
 - n_submit_timestamp (number; default -1):
-    Last time that `Enter` was pressed.
+    Last time that `Enter` was pressed. Only updates if
+    submit_on_enter is True.
 
 - name (string; optional):
     Name of the element. For example used by the server to identify
     the fields in form submits.
 
 - persisted_props (list of a value equal to: 'value's; default ['value']):
     Properties whose user interactions will persist after refreshing
@@ -196,14 +197,19 @@
 
 - spellcheck (a value equal to: 'true', 'false' | boolean; optional):
     Indicates whether spell checking is allowed for the element.
 
 - style (dict; optional):
     Defines CSS styles which will override styles previously set.
 
+- submit_on_enter (boolean; default True):
+    Whether or not the form should increment the n_submit and
+    n_submit_timestamp props when enter key is pressed. If True, use
+    shift + enter to create a newline. Default: True.
+
 - tabIndex (string | number; optional):
     **DEPRECATED** Use `tabindex` instead  Overrides the browser's
     default tab order and follows the one specified instead.
 
 - tabindex (string | number; optional):
     Overrides the browser's default tab order and follows the one
     specified instead.
@@ -222,18 +228,18 @@
 - wrap (string; optional):
     Indicates whether the text should be wrapped."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_bootstrap_components'
     _type = 'Textarea'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, key=Component.UNDEFINED, value=Component.UNDEFINED, autofocus=Component.UNDEFINED, autoFocus=Component.UNDEFINED, cols=Component.UNDEFINED, disabled=Component.UNDEFINED, form=Component.UNDEFINED, maxlength=Component.UNDEFINED, maxLength=Component.UNDEFINED, minlength=Component.UNDEFINED, minLength=Component.UNDEFINED, name=Component.UNDEFINED, placeholder=Component.UNDEFINED, readonly=Component.UNDEFINED, readOnly=Component.UNDEFINED, required=Component.UNDEFINED, rows=Component.UNDEFINED, wrap=Component.UNDEFINED, accesskey=Component.UNDEFINED, accessKey=Component.UNDEFINED, class_name=Component.UNDEFINED, className=Component.UNDEFINED, contenteditable=Component.UNDEFINED, contentEditable=Component.UNDEFINED, contextmenu=Component.UNDEFINED, contextMenu=Component.UNDEFINED, dir=Component.UNDEFINED, draggable=Component.UNDEFINED, hidden=Component.UNDEFINED, lang=Component.UNDEFINED, spellcheck=Component.UNDEFINED, spellCheck=Component.UNDEFINED, style=Component.UNDEFINED, tabindex=Component.UNDEFINED, tabIndex=Component.UNDEFINED, title=Component.UNDEFINED, size=Component.UNDEFINED, valid=Component.UNDEFINED, invalid=Component.UNDEFINED, n_blur=Component.UNDEFINED, n_blur_timestamp=Component.UNDEFINED, n_submit=Component.UNDEFINED, n_submit_timestamp=Component.UNDEFINED, n_clicks=Component.UNDEFINED, n_clicks_timestamp=Component.UNDEFINED, debounce=Component.UNDEFINED, loading_state=Component.UNDEFINED, persistence=Component.UNDEFINED, persisted_props=Component.UNDEFINED, persistence_type=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'accessKey', 'accesskey', 'autoFocus', 'autofocus', 'className', 'class_name', 'cols', 'contentEditable', 'contenteditable', 'contextMenu', 'contextmenu', 'debounce', 'dir', 'disabled', 'draggable', 'form', 'hidden', 'invalid', 'key', 'lang', 'loading_state', 'maxLength', 'maxlength', 'minLength', 'minlength', 'n_blur', 'n_blur_timestamp', 'n_clicks', 'n_clicks_timestamp', 'n_submit', 'n_submit_timestamp', 'name', 'persisted_props', 'persistence', 'persistence_type', 'placeholder', 'readOnly', 'readonly', 'required', 'rows', 'size', 'spellCheck', 'spellcheck', 'style', 'tabIndex', 'tabindex', 'title', 'valid', 'value', 'wrap']
+    def __init__(self, id=Component.UNDEFINED, key=Component.UNDEFINED, value=Component.UNDEFINED, autofocus=Component.UNDEFINED, autoFocus=Component.UNDEFINED, cols=Component.UNDEFINED, disabled=Component.UNDEFINED, form=Component.UNDEFINED, maxlength=Component.UNDEFINED, maxLength=Component.UNDEFINED, minlength=Component.UNDEFINED, minLength=Component.UNDEFINED, name=Component.UNDEFINED, placeholder=Component.UNDEFINED, readonly=Component.UNDEFINED, readOnly=Component.UNDEFINED, required=Component.UNDEFINED, rows=Component.UNDEFINED, wrap=Component.UNDEFINED, accesskey=Component.UNDEFINED, accessKey=Component.UNDEFINED, class_name=Component.UNDEFINED, className=Component.UNDEFINED, contenteditable=Component.UNDEFINED, contentEditable=Component.UNDEFINED, contextmenu=Component.UNDEFINED, contextMenu=Component.UNDEFINED, dir=Component.UNDEFINED, draggable=Component.UNDEFINED, hidden=Component.UNDEFINED, lang=Component.UNDEFINED, spellcheck=Component.UNDEFINED, spellCheck=Component.UNDEFINED, style=Component.UNDEFINED, tabindex=Component.UNDEFINED, tabIndex=Component.UNDEFINED, title=Component.UNDEFINED, size=Component.UNDEFINED, valid=Component.UNDEFINED, invalid=Component.UNDEFINED, n_blur=Component.UNDEFINED, n_blur_timestamp=Component.UNDEFINED, n_submit=Component.UNDEFINED, n_submit_timestamp=Component.UNDEFINED, submit_on_enter=Component.UNDEFINED, n_clicks=Component.UNDEFINED, n_clicks_timestamp=Component.UNDEFINED, debounce=Component.UNDEFINED, loading_state=Component.UNDEFINED, persistence=Component.UNDEFINED, persisted_props=Component.UNDEFINED, persistence_type=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'accessKey', 'accesskey', 'autoFocus', 'autofocus', 'className', 'class_name', 'cols', 'contentEditable', 'contenteditable', 'contextMenu', 'contextmenu', 'debounce', 'dir', 'disabled', 'draggable', 'form', 'hidden', 'invalid', 'key', 'lang', 'loading_state', 'maxLength', 'maxlength', 'minLength', 'minlength', 'n_blur', 'n_blur_timestamp', 'n_clicks', 'n_clicks_timestamp', 'n_submit', 'n_submit_timestamp', 'name', 'persisted_props', 'persistence', 'persistence_type', 'placeholder', 'readOnly', 'readonly', 'required', 'rows', 'size', 'spellCheck', 'spellcheck', 'style', 'submit_on_enter', 'tabIndex', 'tabindex', 'title', 'valid', 'value', 'wrap']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'accessKey', 'accesskey', 'autoFocus', 'autofocus', 'className', 'class_name', 'cols', 'contentEditable', 'contenteditable', 'contextMenu', 'contextmenu', 'debounce', 'dir', 'disabled', 'draggable', 'form', 'hidden', 'invalid', 'key', 'lang', 'loading_state', 'maxLength', 'maxlength', 'minLength', 'minlength', 'n_blur', 'n_blur_timestamp', 'n_clicks', 'n_clicks_timestamp', 'n_submit', 'n_submit_timestamp', 'name', 'persisted_props', 'persistence', 'persistence_type', 'placeholder', 'readOnly', 'readonly', 'required', 'rows', 'size', 'spellCheck', 'spellcheck', 'style', 'tabIndex', 'tabindex', 'title', 'valid', 'value', 'wrap']
+        self.available_properties = ['id', 'accessKey', 'accesskey', 'autoFocus', 'autofocus', 'className', 'class_name', 'cols', 'contentEditable', 'contenteditable', 'contextMenu', 'contextmenu', 'debounce', 'dir', 'disabled', 'draggable', 'form', 'hidden', 'invalid', 'key', 'lang', 'loading_state', 'maxLength', 'maxlength', 'minLength', 'minlength', 'n_blur', 'n_blur_timestamp', 'n_clicks', 'n_clicks_timestamp', 'n_submit', 'n_submit_timestamp', 'name', 'persisted_props', 'persistence', 'persistence_type', 'placeholder', 'readOnly', 'readonly', 'required', 'rows', 'size', 'spellCheck', 'spellcheck', 'style', 'submit_on_enter', 'tabIndex', 'tabindex', 'title', 'valid', 'value', 'wrap']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         super(Textarea, self).__init__(**args)
```

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Toast.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Toast.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/Tooltip.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/Tooltip.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/__init__.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/dash_bootstrap_components.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -10268,15 +10268,15 @@
                         is_open: !1
                     }))
                 },
                 D = function() {
                     !x.current && N.current ? (N.current = clearTimeout(N.current), R()) : x.current && (clearTimeout(w.current), w.current = setTimeout(R, d.hide))
                 },
                 L = function() {
-                    x.current || (N.current = clearTimeout(N.current), _(!0), m && E && m({
+                    x.current || (N.current = clearTimeout(N.current), _(!0), m && E.current && m({
                         is_open: !0
                     }))
                 },
                 I = function() {
                     x.current && w.current ? (w.current = clearTimeout(w.current), L()) : x.current || (clearTimeout(N.current), N.current = setTimeout(L, d.show))
                 },
                 $ = function(e) {
@@ -11869,15 +11869,15 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
         const cm = lm;
-        var um = ["value", "n_clicks", "n_blur", "n_submit", "setProps", "className", "class_name", "invalid", "valid", "size", "debounce", "loading_state", "autoFocus", "autofocus", "maxLength", "maxlength", "minLength", "minlength", "readOnly", "readonly", "accessKey", "accesskey", "contentEditable", "contenteditable", "contextMenu", "contextmenu", "spellCheck", "spellcheck", "tabIndex", "tabindex"],
+        var um = ["value", "n_clicks", "n_blur", "n_submit", "setProps", "className", "class_name", "invalid", "valid", "size", "debounce", "loading_state", "autoFocus", "autofocus", "maxLength", "maxlength", "minLength", "minlength", "readOnly", "readonly", "accessKey", "accesskey", "contentEditable", "contenteditable", "contextMenu", "contextmenu", "spellCheck", "spellcheck", "tabIndex", "tabindex", "submit_on_enter"],
             dm = function(t) {
                 var n = t.value,
                     r = t.n_clicks,
                     a = t.n_blur,
                     s = t.n_submit,
                     c = t.setProps,
                     u = t.className,
@@ -11901,42 +11901,43 @@
                     T = t.contenteditable,
                     S = t.contextMenu,
                     R = t.contextmenu,
                     D = t.spellCheck,
                     L = t.spellcheck,
                     I = t.tabIndex,
                     $ = t.tabindex,
-                    A = o(t, um),
-                    M = Se((0, i.useState)(n || ""), 2),
-                    F = M[0],
-                    B = M[1];
+                    A = t.submit_on_enter,
+                    M = o(t, um),
+                    F = Se((0, i.useState)(n || ""), 2),
+                    B = F[0],
+                    z = F[1];
                 (0, i.useEffect)((function() {
-                    n !== F && B(n || "")
+                    n !== B && z(n || "")
                 }), [n]);
-                var z = b()(d || u, p && "is-invalid", f && "is-valid", !!g && "form-control-".concat(g), "form-control");
+                var K = b()(d || u, p && "is-invalid", f && "is-valid", !!g && "form-control-".concat(g), "form-control");
                 return l().createElement("textarea", e({
-                    value: F,
-                    className: z,
+                    value: B,
+                    className: K,
                     onChange: function(e) {
                         var t = e.target.value;
-                        B(t), !y && c && c({
+                        z(t), !y && c && c({
                             value: t
                         })
                     },
                     onBlur: function(e) {
                         if (c) {
                             var t = {
                                 n_blur: a + 1,
                                 n_blur_timestamp: Date.now()
                             };
                             y && (t.value = e.target.value), c(t)
                         }
                     },
                     onKeyPress: function(e) {
-                        if (c && "Enter" === e.key && !e.shiftKey) {
+                        if (A && c && "Enter" === e.key && !e.shiftKey) {
                             e.preventDefault();
                             var t = {
                                 n_submit: s + 1,
                                 n_submit_timestamp: Date.now()
                             };
                             y && (t.value = e.target.value), c(t)
                         }
@@ -11952,15 +11953,15 @@
                     minLength: N || w,
                     readOnly: j || E,
                     accessKey: P || k,
                     contentEditable: T || C,
                     contextMenu: R || S,
                     spellCheck: L || D,
                     tabIndex: $ || I
-                }, m(["n_blur_timestamp", "n_submit_timestamp", "persistence", "persistence_type", "persisted_props"], A), {
+                }, m(["n_blur_timestamp", "n_submit_timestamp", "persistence", "persistence_type", "persisted_props"], M), {
                     "data-dash-is-loading": h && h.is_loading || void 0
                 }))
             };
         dm.propTypes = {
             id: u().string,
             key: u().string,
             value: u().string,
@@ -12002,14 +12003,15 @@
             size: u().string,
             valid: u().bool,
             invalid: u().bool,
             n_blur: u().number,
             n_blur_timestamp: u().number,
             n_submit: u().number,
             n_submit_timestamp: u().number,
+            submit_on_enter: u().bool,
             n_clicks: u().number,
             n_clicks_timestamp: u().number,
             debounce: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
@@ -12023,15 +12025,16 @@
             n_submit: 0,
             n_submit_timestamp: -1,
             n_clicks: 0,
             n_clicks_timestamp: -1,
             debounce: !1,
             persisted_props: ["value"],
             persistence_type: "local",
-            value: ""
+            value: "",
+            submit_on_enter: !0
         };
         const pm = dm,
             fm = {
                 [z]: "showing",
                 [H]: "showing show"
             },
             mm = i.forwardRef(((e, t) => (0, _.jsx)(mt, {
```

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_components/metadata.json` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999798992281304%*

 * *Differences: {"'src/components/input/Textarea.js'": "{'props': {'n_submit': {'description': 'Number of times "*

 * *                                       'the `Enter` key was pressed while the textarea had focus. '*

 * *                                       "Only\\nupdates if submit_on_enter is True.'}, "*

 * *                                       "'n_submit_timestamp': {'description': 'Last time that "*

 * *                                       '`Enter` was pressed. Only updates if submit_on_enter is '*

 * *                                 […]*

```diff
@@ -6261,26 +6261,26 @@
                 }
             },
             "n_submit": {
                 "defaultValue": {
                     "computed": false,
                     "value": "0"
                 },
-                "description": "Number of times the `Enter` key was pressed while the textarea had focus.",
+                "description": "Number of times the `Enter` key was pressed while the textarea had focus. Only\nupdates if submit_on_enter is True.",
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             },
             "n_submit_timestamp": {
                 "defaultValue": {
                     "computed": false,
                     "value": "-1"
                 },
-                "description": "Last time that `Enter` was pressed.",
+                "description": "Last time that `Enter` was pressed. Only updates if submit_on_enter is True.",
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             },
             "name": {
                 "description": "Name of the element. For example used by the server to identify the fields in form submits.",
@@ -6524,14 +6524,25 @@
             "style": {
                 "description": "Defines CSS styles which will override styles previously set.",
                 "required": false,
                 "type": {
                     "name": "object"
                 }
             },
+            "submit_on_enter": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "true"
+                },
+                "description": "Whether or not the form should increment the n_submit and n_submit_timestamp props\nwhen enter key is pressed. If True, use shift + enter to create a newline. Default: True",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
             "tabIndex": {
                 "description": "**DEPRECATED** Use `tabindex` instead\n\nOverrides the browser's default tab order and follows the one specified instead.",
                 "required": false,
                 "type": {
                     "name": "union",
                     "value": [
                         {
```

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/_table.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/_table.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components/themes.py` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components/themes.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/PKG-INFO` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-bootstrap-components
-Version: 1.6.1rc1
+Version: 1.6.1rc2
 Summary: Bootstrap themed components for use in Plotly Dash
 Home-page: https://dash-bootstrap-components.opensource.faculty.ai/
 Author: Faculty
 Author-email: opensource@faculty.ai
 License: Apache Software License
 Project-URL: Bug Reports, https://github.com/facultyai/dash-bootstrap-components/issues
 Project-URL: Source, https://github.com/facultyai/dash-bootstrap-components/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.1rc1
+Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.1rc2
 Summary: Bootstrap themed components for use in Plotly Dash Home-page: https://
 dash-bootstrap-components.opensource.faculty.ai/ Author: Faculty Author-email:
 opensource@faculty.ai License: Apache Software License Project-URL: Bug
 Reports, https://github.com/facultyai/dash-bootstrap-components/issues Project-
 URL: Source, https://github.com/facultyai/dash-bootstrap-components/
 Classifier: Framework :: Dash Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `dash_bootstrap_components-1.6.1rc1/dash_bootstrap_components.egg-info/SOURCES.txt` & `dash_bootstrap_components-1.6.1rc2/dash_bootstrap_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/landing-page.md` & `dash_bootstrap_components-1.6.1rc2/landing-page.md`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/setup.cfg` & `dash_bootstrap_components-1.6.1rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/setup.py` & `dash_bootstrap_components-1.6.1rc2/setup.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/tests/test_components_as_props.py` & `dash_bootstrap_components-1.6.1rc2/tests/test_components_as_props.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/tests/test_navlink.py` & `dash_bootstrap_components-1.6.1rc2/tests/test_navlink.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/tests/test_popover.py` & `dash_bootstrap_components-1.6.1rc2/tests/test_popover.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/tests/test_positional_args.py` & `dash_bootstrap_components-1.6.1rc2/tests/test_positional_args.py`

 * *Files identical despite different names*

### Comparing `dash_bootstrap_components-1.6.1rc1/tests/test_tooltip.py` & `dash_bootstrap_components-1.6.1rc2/tests/test_tooltip.py`

 * *Files identical despite different names*

