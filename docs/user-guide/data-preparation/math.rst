Math
==========

Fire Insights provide processors for Mathematical computation


Math Processors in Fire Insights
----------------------------------------


.. list-table:: Math Processors
   :widths: 30 70
   :header-rows: 1

   * - Title
     - Description
   * - Math Expression
     - It computes new values using Math Expression
   * - Math Functions Multiple
     - It computes new values by application of Maths functions on incoming columns
 
 
Math Expression
----------------------------------------

Below is a sample workflow which contains ``Math Expression`` processor in Fire Insights. It demonstrates usage of ``Math Expression`` node to compute new column value using Math Expressions.

It does following processing of data:

*	Reads incoming Dataset.
*	Computes new column value by evaluating expressions using ``Math Expression`` node.
*	Prints output dataset with new columns computed by evaluating math expressions.

.. figure:: ../../_assets/user-guide/data-preparation/math/mathexp-workflow.png
   :alt: math_userguide
   :width: 90%
   
**Incoming dataset**

.. figure:: ../../_assets/user-guide/data-preparation/math/mathexp-incoming-dataset.png
   :alt: math_userguide
   :width: 90%
   
**Math Expression Node configuration**

*	``Math Expression`` node is configured as below.
*	Input of this node are the incoming dataset.
*	Column that needs to list computed values in the output is to be entered in ``Output Column`` box.
*	Mathematical Expression that needs to evaluated to compute new colum in the output is to be entered in ``Math Expression`` box.
*	A new ``Key Value Array`` row needs to be added for each additional Math Expression.
*	Output of this node would display dataset with new columns computed by evaluating math expressions.

.. figure:: ../../_assets/user-guide/data-preparation/math/mathexp-config.png
   :alt: math_userguide
   :width: 90%
   
**Math Expression Node output**

Output of ``Math Expression`` node displaying dataset with new columns computed by evaluating math expressions.

.. figure:: ../../_assets/user-guide/data-preparation/math/mathexp-printnode-output.png
   :alt: math_userguide
   :width: 90%       	    
   

Math Functions Multiple
----------------------------------------

Below is a sample workflow which contains ``Math Functions Multiple`` processor in Fire Insights. It demonstrates usage of ``Math Functions Multiple`` node to compute values using selected Math function.

It does following processing of data:

*	Reads incoming Dataset.
*	Computes values by application of selected Math function on incoming columns using ``Math Functions Multiple`` node.
*	Prints output dataset with new columns computed using math functions.

.. figure:: ../../_assets/user-guide/data-preparation/math/mathfuncmul-workflow.png
   :alt: math_userguide
   :width: 90%
   
**Incoming dataset**

.. figure:: ../../_assets/user-guide/data-preparation/math/mathfuncmul-incoming-dataset.png
   :alt: math_userguide
   :width: 90%
   
**Math Functions Multiple Node configuration**

*	``Math Functions Multiple`` node is configured as below.
*	Input of this node are the incoming dataset.
*	Incoming Column on which math function needs to be applied to compute new value is to be selected in ``Columns`` list.
*	Function that needs to be applied on incoming column to compute new value is to be selected in ``Function`` list.
*	``Replace Existing Cols`` needs to be selected as true if new column is to replace existing incoming column in the output.
*	Scale that needs to be applied while using math function is to be entered in ``Scale`` box. In this example ``Tax_Amt`` value is to be raised by a Power of 2 hence scale is entered as 2. In another calculation ``List_Price`` value is to be rounded to 1 decimal place hence Scale is selected as 1.
*	A new ``Variables List`` row needs to be added for each additional computation.
*	Output of this node would display dataset with new columns computed using math functions.

.. figure:: ../../_assets/user-guide/data-preparation/math/mathfuncmul-config.png
   :alt: math_userguide
   :width: 90%
   
**Math Functions Multiple Node output**

Output of ``Math Functions Multiple`` node displaying dataset with new columns computed using math functions.

.. figure:: ../../_assets/user-guide/data-preparation/math/mathfuncmul-printnode-output.png
   :alt: math_userguide
   :width: 90%       	    
   
