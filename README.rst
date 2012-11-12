===========================
 jqPlot Highlighter Plugin
===========================

This is a modification of the highlighter plugin for jqPlot with a few improvements for tooltips:

* tooltips for pie charts, which can be set to custom positions.
* new positioning options for tooltips on bar charts, so they stay on visible area while zooming.

Original files hosted in `Bitbucket <https://bitbucket.org/cleonello/jqplot/>`_.


How to use it
=============

To use this plugin, first include the js file in your source: ::

 <script type="text/javascript" src="plugins/jqplot.highlighter.js"></script>

Pie charts
----------

To use the tooltips for pie charts, you just have to set the highlighter's ``tooltipAxes`` property to *pieref*.
You can also set the tooltip positions by setting the (new) ``tooltipAxisX`` and ``tooltipAxisY`` properties.

::

	highlighter: {
		show:true,
		sizeAdjust: 10,
		tooltipLocation: 'n',
		tooltipAxes: 'pieref',
		tooltipAxisX: 60,
		tooltipAxisY: 90,
		useAxesFormatters: false,
	}


Bar charts
----------

To use the new positioning options for tooltips on bar charts, set the highlighter's ``tooltipAxex`` property to *yref*.

::

	highlighter: {
		show:true,
		sizeAdjust: 10,
		tooltipLocation: 'n',
		tooltipAxes: 'yref',
		useAxesFormatters: false,
	}

More information
================

:Date: 05-14-2012
:Author:
  Lucía González - Tryolabs <lucia@tryolabs.com>
:jqPlot Author: 
  Chris Leonello - <chris@jqplot.com>
:Website:
  https://github.com/tryolabs/jqplot-highlighter
