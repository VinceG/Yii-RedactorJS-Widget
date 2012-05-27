Yii-RedactorJS-Widget
=====================

Yii Widget for the WYSIWYG RedactorJS editor

- [Project Page](http://redactorjs.com/)
- [Examples](http://redactorjs.com/examples/)
- [Documentation](http://redactorjs.com/docs/)

Requirements
=====================

- JQuery > 1.7.1
- Browser:
 - Firefox 3+
 - Safari 4+
 - Chrome 4+
 - Opera 10+
 - IE 7+

Installation
=====================

1. Download or Clone the files
2. Extract into the widgets folder or extensions folder

Usage
===================

Using with a model
------------------

~~~
$this->widget('application.widgets.redactorjs.Redactor', array( 'model' => $model, 'attribute' => 'some_attribute' ));
~~~

Using with a model and a mini toolbar and different language
------------------

~~~
$this->widget('application.widgets.redactorjs.Redactor', array( 'lang' => 'de', 'toolbar' => 'mini', 'model' => $model, 'attribute' => 'some_attribute' ));
~~~

- There are two toolbars supported right now: default & mini. By default the widget will load the 'default' toolbar.
- Supported languages currently: de, en, fr, lv, pl, pt_br, ru, ua

Using with a model and custom toolbar options
------------------

~~~
$this->widget('application.widgets.redactorjs.Redactor', array( 'editorOptions' => array('autoresize' => true, 'fixed' => true), 'model' => $model, 'attribute' => 'some_attribute' ));
~~~

- Referrer to the redactorjs API for the list of supported elements. [View Docs](http://redactorjs.com/docs/settings/)

Using with a name and value
------------------

~~~
$this->widget('application.widgets.redactorjs.Redactor', array( 'name' => 'some name', 'value' => 'some value' ));
~~~


Authors
==================

Vincent Gabriel <http://vadimg.com>
