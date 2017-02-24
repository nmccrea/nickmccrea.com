---
layout:     default
permalink:  /about/
style-id:   about-page
title:      About
---

![Nick McCrea]( {% asset_path 'nick-mccrea-headshot.jpg' %} ){:width="280px" :height="280px"}

<hr />

# About Me

My name is Nick McCrea

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum tristique turpis malesuada blandit mattis. In ut nunc at metus sagittis cursus. Fusce mauris purus, consectetur quis hendrerit et, maximus vel urna. Suspendisse rhoncus magna vel orci vehicula, in malesuada erat vestibulum. Donec ultricies, felis et tincidunt fringilla, sem nulla rhoncus enim, nec maximus urna odio sed nibh. Donec vehicula dui egestas eros sagittis, nec aliquam lectus hendrerit. Phasellus ut risus urna. Donec luctus nunc sed nunc venenatis tempor.

Mauris tempor dolor ut mauris suscipit, eget varius purus pulvinar. Suspendisse egestas et arcu sed dictum. Morbi bibendum, tellus ac lacinia pellentesque, turpis purus convallis mi, quis porttitor neque libero non metus. Cras eu lorem accumsan, dignissim tellus ut, porta urna. Phasellus vestibulum libero commodo tortor tincidunt posuere. In luctus justo non auctor lacinia. Cras at laoreet leo, porta elementum nisl. Aenean eget tincidunt nisi. Curabitur tincidunt pellentesque fringilla. Vivamus imperdiet justo sed nunc bibendum, nec ornare nulla venenatis. Aliquam ligula neque, fringilla vitae venenatis ac, vestibulum ac dui. Phasellus odio enim, aliquam ut odio eget, ornare eleifend eros. Proin rutrum turpis mi, et pulvinar eros eleifend vitae.

Curabitur sapien odio, facilisis at leo id, gravida congue lorem. Duis et ullamcorper dui. Suspendisse blandit neque quis metus bibendum laoreet. Integer bibendum, odio sed faucibus lobortis, lorem felis vestibulum ex, tincidunt faucibus augue erat quis massa. Mauris blandit sodales massa a fringilla. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Nulla aliquam tortor vitae ipsum rutrum, in tincidunt dui sodales.

## This is an H2 Heading

Donec et ultrices tellus. Quisque sodales enim arcu, eu posuere diam congue eget. Sed ut facilisis felis, sed malesuada dui. Nunc molestie ornare tincidunt. Fusce volutpat porttitor tincidunt. Donec sit amet nulla laoreet, elementum ipsum vel, consequat augue. Phasellus sagittis odio id dolor fringilla, ut tristique sapien volutpat. Vivamus cursus ornare hendrerit. Nulla eget vulputate lorem. Phasellus semper ac leo a pellentesque. Suspendisse fringilla in nisl vitae scelerisque. Mauris venenatis viverra feugiat. Nullam molestie eros ac sollicitudin accumsan.

> This is a block quote. Behold the quote in a block. Viva la quotacion bloqué.

Sed at nulla ut erat lacinia finibus. Aliquam quis luctus mauris, a fermentum erat. Sed convallis interdum urna nec dapibus. Nullam et urna ac lacus sollicitudin pellentesque in a tortor. Maecenas venenatis ex et est viverra, at dapibus felis sagittis. Sed libero dolor, imperdiet at luctus id, lobortis vitae purus. Aliquam euismod urna a dui tincidunt fermentum.

Duis volutpat augue sit amet nisi volutpat, faucibus porttitor nisl pretium. Donec pharetra eros turpis, et tincidunt urna scelerisque id. Mauris eu tellus vitae justo mollis aliquet ac a neque. Praesent ultrices ac risus a euismod. Fusce tempus laoreet facilisis. Nam ut accumsan magna. Fusce justo quam, fermentum sit amet aliquet non, interdum non ante. Morbi convallis vel augue vitae vehicula. Sed commodo placerat faucibus.

### This is an H3 Heading

Nunc lobortis nibh eu erat aliquam, eget semper lacus dapibus. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus fringilla urna vitae mauris eleifend, quis auctor ex iaculis. Suspendisse aliquam, mi in mollis rutrum, lorem libero porttitor metus, sed vulputate enim turpis eu dui. Pellentesque varius diam quis est sagittis, vulputate vestibulum ex consectetur. Aliquam erat volutpat. Integer rhoncus arcu condimentum, vehicula tortor vulputate, dapibus velit. Phasellus at ante tincidunt, varius dui faucibus, blandit nibh.

Here is some `inline code` to style.

~~~ ruby
class User
  ROLES = [ 'admin', 'employee', 'employer' ]

  has_one :employee, dependent: :destroy
  has_one :employer, dependent: :destroy

  validates_associated :employee
  validates_associated :employer

  validate :role_associations

  private def role_associations
    if    is_admin?;      admin_associations
    elsif is_employee?;   employee_associations
    elsif is_employer?;   employer_associations
    else
      errors[:role] << "User role is not defined."
    end
  end

  private def admin_associations
    errors[:employee] << "Admin user may not own a Employee." if self.employee
    errors[:employer] << "Admin user may not own a Employer." if self.employer
  end

  private def employee_associations
    errors[:employee] << "Employee user must own a Employee." unless self.employee
    errors[:employer] << "Employee user may not own a Employer." if self.employer
  end

  private def employer_associations
    errors[:employer] << "Employer user must own a Employer." unless self.employer
    errors[:employee] << "Employer user may not own a Employee." if self.employee
  end

  ##
  # Indicate whether this user is an admin.

  def is_admin?
    self.role == 'admin'
  end

  ##
  # Indicate whether this user is a Employee.

  def is_employee?
    self.role == 'employee'
  end

  ##
  # Indicate whether this user is a Employer.

   def is_employer?
     self.role == 'employer'
  end
end
~~~

Vestibulum urna quam, ultrices sed odio quis, commodo rutrum tellus. Mauris ultricies dolor sed leo varius, ut varius ante aliquam. Praesent porta sodales nisi, eu malesuada tellus ullamcorper sit amet. Morbi a nisl ipsum. Mauris luctus sem at est porta ultricies. Vivamus ultrices quis neque quis venenatis. Praesent a lobortis libero. Sed vitae elementum odio. Phasellus a ullamcorper libero. Suspendisse ullamcorper a neque at varius.

Praesent ultricies fermentum libero, quis tincidunt mauris ultrices in. Sed posuere non nunc nec molestie. Mauris scelerisque nunc sit amet turpis finibus efficitur. Morbi id neque malesuada, lobortis nisi quis, condimentum justo. Curabitur sed augue ut diam ultricies dictum. Nullam ut leo magna. Aliquam sollicitudin lectus quis ultricies tincidunt. Cras lacus tortor, iaculis nec ullamcorper in, eleifend vel odio. Pellentesque feugiat imperdiet nunc, in imperdiet mauris. Suspendisse potenti.

#### This is an H4 Heading

Donec nec nibh sit amet dolor rutrum laoreet nec vel mauris. Suspendisse vitae consequat sem. Phasellus nulla massa, porta eu magna a, vehicula tincidunt arcu. Aliquam in nisl semper, feugiat eros vel, tempus sem. Phasellus sollicitudin ex in diam vestibulum, ac blandit velit ultricies. Curabitur porttitor nibh eu laoreet tristique. Suspendisse sed elit imperdiet, tempor urna nec, scelerisque nisi. Cras sit amet nulla fringilla, malesuada mauris sit amet, bibendum turpis. Nunc ante neque, commodo a orci nec, placerat hendrerit nisi. Nam non sagittis mauris.