<script>
  import { TextField, Row, Col } from 'sveltfy/src';

  const titleRules = [(v) => !!v || 'Required'];
  const emailRules = [
    (v) => !!v || 'Required',
    (v) => v.length <= 25 || 'Max 25 characters',
    (v) => {
      const pattern = /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
      return pattern.test(v) || 'Invalid e-mail.';
    },
  ];
</script>

<Row>
  <Col>
    <TextField counter="20" maxlength="20" rules={titleRules}>Title</TextField>
  </Col>
  <Col>
    <TextField counter="25" rules={emailRules}>Email</TextField>
  </Col>
</Row>
