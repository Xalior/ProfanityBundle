<h1>Profanity Filter Bundle</h1>

A symfony bundle to test if a string has a profanity in it.

<b>Straight matching</b>
Checks string for profanity as it is against list of bad words. E.g. badword

<b>Substitution</b>
Checks string for profanity with characters substituted for each letter. E.g. bâdΨ0rd

<b>Obscured</b>
Checks string for profanity obscured with punctuation between. E.g. b|a|d|w|o|r|d

<b>Combinations</b>
Also works with combinations of the above. E.g. b|â|d|Ψ|0|rr|d

<h4>Installation</h4>
<ul>
  <li>
    Install this package via composer.

    <pre>php composer.phar require vangrg/profanity-bundle</pre>
  </li>
  <li>
    Add to your AppKernel.php:

    new Vangrg\ProfanityBundle\VangrgProfanityBundle(),
   </li>
   <li>
      If you want to use a database to store your profanities:

      <pre>php app/console doctrine:schema:update --force</pre>
   </li>
</ul>

