# bangazon-02-methodoverriding
Specializing Derived Classes with Overriding

Bangazon Orientation - Specializing Derived Classes with Overriding

Instructions

Override

Choose one of the general methods that you created in the Department class for overriding. For example, the meet() method which handles the logic of how teammates in that department gather for a meeting.
Override that method in all of your derived classes, giving each a more specialized implementation. For example, you could output a different meeting place for each department.
Override, but use parent

Now make a method on Department named get_budget(). It will set, and return, the base budget that each department gets each year. You pick what that number is.
Override that method in each of the derived classes.
Make sure you invoke the parent class' overridden method with the super keyword (e.g. super().get_budget()). That will set the base budget.
Now add, or subtract, from that base budget inside the derived class' override method to adjust that specific department's budget.
class Department(object):
  """Parent class for all departments

  Methods: __init__, get_name, get_supervisor, meet
  """

  def meet():
    print("Everyone meet in {}'s office".format(self.supervisor))
class Development(object):
  """Software development department

  Methods: __init__, get_name, get_supervisor, meet
  """

  def meet():
    """This overrides the base meet() method completely"""
    
    print("Everyone meet in the server room")
