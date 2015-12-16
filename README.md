# Table2li

A HTML to HTML converter. Converts from table to list.

## Installation

    $ gem install table2li

## Usage

TODO: Write usage instructions here

## Exapmle

### Formal

From:

<table>
  <thead>
    <tr>
      <th>id</th>
      <th>name</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Ai</td>
      <td>Me.</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Go</td>
      <td>You.</td>
    </tr>
  </tbody>
</table>

To:

<ul>
<li>1<ul><li>id<ul><li>1</li></ul>
</li></ul>
<ul><li>name<ul><li>Ai</li></ul>
</li></ul>
<ul><li>description<ul><li>Me.</li></ul>
</li></ul>
</li>
<li>2<ul><li>id<ul><li>5</li></ul>
</li></ul>
<ul><li>name<ul><li>Go</li></ul>
</li></ul>
<ul><li>description<ul><li>You.</li></ul>
</li></ul>
</li>
</ul>

### Simple

From:

<table>
  <tr>
    <th>id</th>
    <th>name</th>
    <th>description</th>
  </tr>
  <tr>
    <td>1</td>
    <td>Ai</td>
    <td>Me.</td>
  </tr>
  <tr>
    <td>5</td>
    <td>Go</td>
    <td>You.</td>
  </tr>
</table>

To:

<ul>
<li>1<ul><li>id<ul><li>1</li></ul>
</li></ul>
<ul><li>name<ul><li>Ai</li></ul>
</li></ul>
<ul><li>description<ul><li>Me.</li></ul>
</li></ul>
</li>
<li>2<ul><li>id<ul><li>5</li></ul>
</li></ul>
<ul><li>name<ul><li>Go</li></ul>
</li></ul>
<ul><li>description<ul><li>You.</li></ul>
</li></ul>
</li>
</ul>

### No TH

From:

<table>
  <tr>
    <td>1</td>
    <td>Ai</td>
    <td>Me.</td>
  </tr>
  <tr>
    <td>5</td>
    <td>Go</td>
    <td>You.</td>
  </tr>
</table>

To:

<ul>
<li>1<ul><li>1</li></ul>
<ul><li>Ai</li></ul>
<ul><li>Me.</li></ul>
</li>
<li>2<ul><li>5</li></ul>
<ul><li>Go</li></ul>
<ul><li>You.</li></ul>
</li>
</ul>

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/myokoym/table2li.

